---
UID: NF:dbgeng.IDebugControl.GetSupportedProcessorTypes
title: IDebugControl::GetSupportedProcessorTypes (dbgeng.h)
description: Learn how the GetSupportedProcessorTypes method returns the processor types supported by the debugger engine.
old-location: debugger\getsupportedprocessortypes.htm
tech.root: debugger
ms.date: 05/03/2018
keywords: ["IDebugControl::GetSupportedProcessorTypes"]
ms.keywords: GetSupportedProcessorTypes, GetSupportedProcessorTypes method [Windows Debugging], GetSupportedProcessorTypes method [Windows Debugging],IDebugControl interface, GetSupportedProcessorTypes method [Windows Debugging],IDebugControl2 interface, GetSupportedProcessorTypes method [Windows Debugging],IDebugControl3 interface, IDebugControl interface [Windows Debugging],GetSupportedProcessorTypes method, IDebugControl.GetSupportedProcessorTypes, IDebugControl2 interface [Windows Debugging],GetSupportedProcessorTypes method, IDebugControl2::GetSupportedProcessorTypes, IDebugControl3 interface [Windows Debugging],GetSupportedProcessorTypes method, IDebugControl3::GetSupportedProcessorTypes, IDebugControl::GetSupportedProcessorTypes, IDebugControl_555eef6a-df68-4f94-9cfa-dc31aee27014.xml, dbgeng/IDebugControl2::GetSupportedProcessorTypes, dbgeng/IDebugControl3::GetSupportedProcessorTypes, dbgeng/IDebugControl::GetSupportedProcessorTypes, debugger.getsupportedprocessortypes
req.header: dbgeng.h
req.include-header: Dbgeng.h
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
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
 - IDebugControl::GetSupportedProcessorTypes
 - dbgeng/IDebugControl::GetSupportedProcessorTypes
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - dbgeng.h
api_name:
 - IDebugControl::GetSupportedProcessorTypes
---

# IDebugControl::GetSupportedProcessorTypes


## -description

The <b>GetSupportedProcessorTypes</b> method returns the processor types supported by the <a href="/windows-hardware/drivers/debugger/introduction">debugger engine</a>.

## -parameters

### -param Start 

[in]
Specifies the index of the first processor type to return.  The supported processor types are indexed by the numbers zero through the number of supported processor types minus one.  The number of supported processor types can be found using <a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugcontrol3-getnumbersupportedprocessortypes">GetNumberSupportedProcessorTypes</a>.

### -param Count 

[in]
Specifies the number of processor types to return.

### -param Types 

[out]
Receives the list of processor types.  The number of elements this array holds is <i>Count</i>.  For a description of the processor types, see <a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugcontrol3-getactualprocessortype">GetActualProcessorType</a>.

## -returns

This method may also return error values.  See <a href="/windows-hardware/drivers/debugger/hresult-values">Return Values</a> for more details.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
</table>

## -remarks

For more information, see <a href="/windows-hardware/drivers/debugger/target-information">Target Information</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugcontrol3-getnumbersupportedprocessortypes">GetNumberSupportedProcessorTypes</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugcontrol3-getprocessortypenames">GetProcessorTypeNames</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugcontrol">IDebugControl</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugcontrol2">IDebugControl2</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugcontrol3">IDebugControl3</a>

