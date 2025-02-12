---
UID: NF:wdm.KeRaiseIrqlToDpcLevel
title: KeRaiseIrqlToDpcLevel function (wdm.h)
description: Learn how the KeRaiseIrqlToDpcLevel routine raises the hardware priority to IRQL = DISPATCH_LEVEL, thereby masking off interrupts of equivalent or lower IRQL on the current processor.
old-location: kernel\keraiseirqltodpclevel.htm
tech.root: kernel
ms.date: 04/30/2018
keywords: ["KeRaiseIrqlToDpcLevel function"]
ms.keywords: KeRaiseIrqlToDpcLevel, KeRaiseIrqlToDpcLevel routine [Kernel-Mode Driver Architecture], k105_64c33a5b-8efa-4d97-9569-2ea68a227d17.xml, kernel.keraiseirqltodpclevel, wdm/KeRaiseIrqlToDpcLevel
req.header: wdm.h
req.include-header: Wdm.h, Ntddk.h
req.target-type: Universal
req.target-min-winverclnt: Available starting with Windows 2000.
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: HwStorPortProhibitedDDIs
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Hal.lib
req.dll: NtosKrnl.exe
req.irql: <= DISPATCH_LEVEL (see Remarks section)
targetos: Windows
req.typenames: 
f1_keywords:
 - KeRaiseIrqlToDpcLevel
 - wdm/KeRaiseIrqlToDpcLevel
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - NtosKrnl.exe
api_name:
 - KeRaiseIrqlToDpcLevel
---

# KeRaiseIrqlToDpcLevel function (wdm.h)


## -description

The **KeRaiseIrqlToDpcLevel** routine raises the hardware priority to IRQL = DISPATCH_LEVEL, thereby masking off interrupts of equivalent or lower IRQL on the current processor.

## -parameters

## -returns

**KeRaiseIrqlToDpcLevel** returns the IRQL at which the call occurred.

## -remarks

Any caller of **KeRaiseIrqlToDpcLevel** should save the returned IRQL value. Every such caller must restore the original IRQL as quickly as possible by passing this returned IRQL in a subsequent call to [KeLowerIrql](nf-wdm-kelowerirql~r1.md).

Callers of **KeRaiseIrqlToDpcLevel** must be running at IRQL <= DISPATCH_LEVEL. Otherwise, a call to this routine causes a bug check.

## -see-also

[KeGetCurrentIrql](nf-wdm-kegetcurrentirql.md)

[KeLowerIrql](nf-wdm-kelowerirql~r1.md)

[KeRaiseIrql](nf-wdm-keraiseirql.md)

