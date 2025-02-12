---
UID: NC:wdfrequest.EVT_WDF_REQUEST_IMPERSONATE
title: EVT_WDF_REQUEST_IMPERSONATE (wdfrequest.h)
description: A driver's EvtRequestImpersonate event callback function performs tasks at the requested impersonation level, such as opening a protected file.
old-location: wdf\evtrequestimpersonate.htm
tech.root: wdf
ms.date: 06/03/2020
keywords: ["EVT_WDF_REQUEST_IMPERSONATE callback function"]
ms.keywords: EVT_WDF_REQUEST_IMPERSONATE, EVT_WDF_REQUEST_IMPERSONATE callback, EvtRequestImpersonate, EvtRequestImpersonate callback function, wdf.evtrequestimpersonate, wdfrequest/EvtRequestImpersonate
req.header: wdfrequest.h
req.include-header: Wdf.h
req.target-type: Universal
req.target-min-winverclnt: Windows 8.1
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 2.0
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
req.typenames: 
f1_keywords:
 - EVT_WDF_REQUEST_IMPERSONATE
 - wdfrequest/EVT_WDF_REQUEST_IMPERSONATE
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - Wdfrequest.h
api_name:
 - EVT_WDF_REQUEST_IMPERSONATE
---

# EVT_WDF_REQUEST_IMPERSONATE callback function


## -description

<p class="CCE_Message">[Applies to UMDF only]</p>

A driver's <i>EvtRequestImpersonate</i> event callback function performs tasks at the requested impersonation level, such as opening a protected file.

## -parameters

### -param Request 

[in]
A handle to a framework request object that represents the I/O request that requires impersonation.

### -param Context 

[in, optional]
A pointer to a context that was previously supplied in the <a href="/windows-hardware/drivers/ddi/wdfrequest/nf-wdfrequest-wdfrequestimpersonate">WdfRequestImpersonate</a> method. This parameter is optional and can be NULL if a context is not required.

## -remarks

User-Mode Driver Framework (UMDF) does not allow a driver's <i>EvtRequestImpersonate</i> callback function to call any of the framework's object methods. This ensures that the driver does not expose the impersonation level to other driver callback functions or other drivers.

The <b>EVT_WDF_REQUEST_IMPERSONATE</b> function type is defined in the Wdfrequest.h header file. To more accurately identify errors when you run the code analysis tools, be sure to add the `_Use_decl_annotations_` annotation to your function definition. The `_Use_decl_annotations_` annotation ensures that the annotations that are applied to the <b>EVT_WDF_REQUEST_IMPERSONATE</b> function type in the header file are used.


The following restrictions also apply: 

 - When the driver calls [**WdfRequestImpersonate**](./nf-wdfrequest-wdfrequestimpersonate.md) with `ImpersonationLevel = SecurityIdentification`, the callback cannot call **LoadLibrary** or perform any action requiring an access check.

 - The same principle applies to DLL delay load. Consider an example in which the driver impersonates at identification level, and the callback calls **GetUserNameW**. Because this API in turn delay loads another DLL and calls **GetUserNameExW**, the initial call might fail with **ERROR_PROC_NOT_FOUND** or **ERROR_BAD_IMPERSONATION_LEVEL**. In such a case, the callback should instead call **GetUserNameExW** directly.


For more information, see <a href="/windows-hardware/drivers/wdf/handling-client-impersonation-in-umdf-drivers">Handling Client Impersonation in UMDF Drivers</a>.


#### Examples

To define an <i>EvtRequestImpersonate</i> callback function, you must first provide a function declaration that identifies the type of callback function you’re defining. Windows provides a set of callback function types for drivers. Declaring a function using the callback function types helps <a href="/windows-hardware/drivers/devtest/code-analysis-for-drivers">Code Analysis for Drivers</a>, <a href="/windows-hardware/drivers/devtest/static-driver-verifier">Static Driver Verifier</a> (SDV), and other verification tools find errors, and it’s a requirement for writing drivers for the Windows operating system.

For example, to define an <i>EvtRequestImpersonate</i> callback function that is named <i>MyRequestImpersonate</i>, use the <b>EVT_WDF_REQUEST_IMPERSONATE</b> type as shown in this code example:

```cpp
EVT_WDF_REQUEST_IMPERSONATE  MyRequestImpersonate;
```

Then, implement your callback function as follows:

```cpp
_Use_decl_annotations_
VOID
 MyRequestImpersonate (
    WDFREQUEST  Request
    PVOID  Context
    )
  {...}
```



For more information about the requirements for function declarations, see <a href="/windows-hardware/drivers/devtest/declaring-functions-by-using-function-role-types-for-kmdf-drivers">Declaring Functions by Using Function Role Types for KMDF Drivers</a>.

For information about _Use_decl_annotations_, see <a href="/cpp/code-quality/annotating-function-behavior">Annotating Function Behavior</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/wdfrequest/nf-wdfrequest-wdfrequestimpersonate">WdfRequestImpersonate</a>

