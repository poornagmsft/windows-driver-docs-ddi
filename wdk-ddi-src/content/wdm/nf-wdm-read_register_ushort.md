---
UID: NF:wdm.READ_REGISTER_USHORT
title: READ_REGISTER_USHORT function (wdm.h)
description: The READ_REGISTER_USHORT function (wdm.h) returns a USHORT value read from the specified register address in resident, mapped device memory.
old-location: kernel\read_register_ushort.htm
tech.root: kernel
ms.date: 09/07/2021
keywords: ["READ_REGISTER_USHORT function"]
ms.keywords: READ_REGISTER_USHORT, READ_REGISTER_USHORT routine [Kernel-Mode Driver Architecture], k103_c2fa06bd-05b9-4fbd-b47c-f264d3ed0bd7.xml, kernel.read_register_ushort, wdm/READ_REGISTER_USHORT
req.header: wdm.h
req.include-header: Wdm.h, Ntddk.h, Ntifs.h, Ioaccess.h, Miniport.h, Wudfwdm.h
req.target-type: Universal
req.target-min-winverclnt: Available starting with Windows 2000.
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
req.lib: NtosKrnl.lib
req.dll: NtosKrnl.exe
req.irql: Any level (see Remarks section)
targetos: Windows
req.typenames: 
f1_keywords:
 - READ_REGISTER_USHORT
 - wdm/READ_REGISTER_USHORT
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - NtosKrnl.exe
api_name:
 - READ_REGISTER_USHORT
---

# READ_REGISTER_USHORT function (wdm.h)


## -description

The **READ_REGISTER_USHORT** routine dereferences the supplied pointer, inserts a memory barrier, and reads a USHORT value from the specified register address.

## -parameters

#### - Register [in]

Pointer to the register address, which must be a mapped range in memory space.

## -returns

<b>READ_REGISTER_USHORT</b> returns the USHORT value read from the specified register address.

## -remarks

This routine inserts a memory barrier into your code. This barrier guarantees that every operation that appears in the source code before the call to this routine will complete before any operation that appears after the call.

For more info about memory barriers, see [**KeMemoryBarrier**](/windows-hardware/drivers/ddi/wdm/nf-wdm-kememorybarrier).

Callers of <b>READ_REGISTER_USHORT</b> can be running at any IRQL, assuming the <i>Register</i> is resident, mapped device memory.

