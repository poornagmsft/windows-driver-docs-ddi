---
UID: NF:wdm.ZwRollbackEnlistment
title: ZwRollbackEnlistment function (wdm.h)
description: Learn how the ZwRollbackEnlistment routine rolls back the transaction that is associated with a specified enlistment.
old-location: kernel\zwrollbackenlistment.htm
tech.root: kernel
ms.date: 04/30/2018
keywords: ["ZwRollbackEnlistment function"]
ms.keywords: NtRollbackEnlistment, ZwRollbackEnlistment, ZwRollbackEnlistment routine [Kernel-Mode Driver Architecture], kernel.zwrollbackenlistment, ktm_ref_6e57f040-d43e-4986-a756-e35e1abc8670.xml, wdm/NtRollbackEnlistment, wdm/ZwRollbackEnlistment
req.header: wdm.h
req.include-header: Wdm.h, Ntifs.h
req.target-type: Universal
req.target-min-winverclnt: Available in Windows Vista and later operating system versions.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: PowerIrpDDis, HwStorPortProhibitedDDIs
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: NtosKrnl.lib
req.dll: NtosKrnl.exe
req.irql: PASSIVE_LEVEL
targetos: Windows
req.typenames: 
f1_keywords:
 - ZwRollbackEnlistment
 - wdm/ZwRollbackEnlistment
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - NtosKrnl.exe
api_name:
 - ZwRollbackEnlistment
---

# ZwRollbackEnlistment function


## -description

The <b>ZwRollbackEnlistment</b> routine rolls back the transaction that is associated with a specified enlistment.

## -parameters

### -param EnlistmentHandle 

[in]
A handle to an <a href="/windows-hardware/drivers/kernel/enlistment-objects">enlistment object</a> that was obtained by a previous call to <a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-ntcreateenlistment">ZwCreateEnlistment</a> or <a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-ntopenenlistment">ZwOpenEnlistment</a>. The handle must have ENLISTMENT_SUBORDINATE_RIGHTS access to the object.

### -param TmVirtualClock 

[in, optional]
A pointer to a <a href="/windows-hardware/drivers/kernel/using-virtual-clock-values">virtual clock value</a>. This parameter is optional and can be <b>NULL</b>.

## -returns

<b>ZwRollbackEnlistment</b> returns STATUS_SUCCESS if the operation succeeds. Otherwise, this routine might return one of the following values: 

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_OBJECT_TYPE_MISMATCH</b></dt>
</dl>
</td>
<td width="60%">
The specified handle is not a handle to an enlistment object.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_INVALID_HANDLE</b></dt>
</dl>
</td>
<td width="60%">
The object handle is invalid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_TRANSACTION_REQUEST_NOT_VALID</b></dt>
</dl>
</td>
<td width="60%">
The enlistment cannot be rolled back.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>STATUS_ACCESS_DENIED</b></dt>
</dl>
</td>
<td width="60%">
The caller does not have appropriate access to the enlistment object.

</td>
</tr>
</table>
 

The routine might return other <a href="/windows-hardware/drivers/kernel/ntstatus-values">NTSTATUS values</a>.

## -remarks

A resource manager can call <b>ZwRollbackEnlistment</b> to roll back a transaction at any time before it calls <a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-ntpreparecomplete">ZwPrepareComplete</a>. 

For more information about <b>ZwRollbackEnlistment</b>, see <a href="/windows-hardware/drivers/kernel/handling-rollback-operations">Handling Rollback Operations</a>.

<b>NtRollbackEnlistment</b> and <b>ZwRollbackEnlistment</b> are two versions of the same Windows Native System Services routine.

For calls from kernel-mode drivers, the <b>Nt<i>Xxx</i></b> and <b>Zw<i>Xxx</i></b> versions of a Windows Native System Services routine can behave differently in the way that they handle and interpret input parameters. For more information about the relationship between the <b>Nt<i>Xxx</i></b> and <b>Zw<i>Xxx</i></b> versions of a routine, see <a href="/windows-hardware/drivers/kernel/using-nt-and-zw-versions-of-the-native-system-services-routines">Using Nt and Zw Versions of the Native System Services Routines</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-tmrollbackenlistment">TmRollbackEnlistment</a>



<a href="/windows-hardware/drivers/kernel/using-nt-and-zw-versions-of-the-native-system-services-routines">Using Nt and Zw Versions of the Native System Services Routines</a>



<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-ntcreateenlistment">ZwCreateEnlistment</a>



<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-ntopenenlistment">ZwOpenEnlistment</a>



<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-ntpreparecomplete">ZwPrepareComplete</a>

