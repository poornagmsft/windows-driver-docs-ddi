---
UID: NF:ntifs.IoStopTimer
title: IoStopTimer function (ntifs.h)
description: The IoStopTimer routine in ntifs.h disables the timer for a specified device object so the driver-supplied IoTimer routine is not called.
old-location: kernel\iostoptimer.htm
tech.root: kernel
ms.date: 04/30/2018
keywords: ["IoStopTimer function"]
ms.keywords: IoStopTimer, IoStopTimer routine [Kernel-Mode Driver Architecture], k104_dfedf779-1137-44c1-ab06-223c3ce6e9c6.xml, kernel.iostoptimer, wdm/IoStopTimer
req.header: ntifs.h
req.include-header: Wdm.h, Ntddk.h, Ntifs.h
req.target-type: Windows
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
req.irql: <= DISPATCH_LEVEL
targetos: Windows
req.typenames: 
f1_keywords:
 - IoStopTimer
 - ntifs/IoStopTimer
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - NtosKrnl.exe
api_name:
 - IoStopTimer
---

# IoStopTimer function (ntifs.h)


## -description

The <b>IoStopTimer</b> routine disables the timer for a specified device object so the driver-supplied <a href="/windows-hardware/drivers/ddi/wdm/nc-wdm-io_timer_routine">IoTimer</a> routine is not called.

## -parameters

### -param DeviceObject 

[in]
Pointer to the device object with which the <a href="/windows-hardware/drivers/ddi/wdm/nc-wdm-io_timer_routine">IoTimer</a> routine is associated.

## -remarks

The driver-supplied <a href="/windows-hardware/drivers/ddi/wdm/nc-wdm-io_timer_routine">IoTimer</a> routine can be reenabled with a call to <b>IoStartTimer</b>.

Do not call <b>IoStopTimer</b> from within the <i>IoTimer</i> routine.

## -see-also

<a href="/windows-hardware/drivers/ddi/wdm/nf-wdm-ioinitializetimer">IoInitializeTimer</a>



<a href="/windows-hardware/drivers/ddi/ntifs/nf-ntifs-iostarttimer">IoStartTimer</a>
