---
UID: NF:ntifs.FsRtlAddMcbEntry
title: FsRtlAddMcbEntry function (ntifs.h)
description: The FsRtlAddMcbEntry function is obsolete.
old-location: ifsk\fsrtladdmcbentry.htm
tech.root: ifsk
ms.date: 04/16/2018
keywords: ["FsRtlAddMcbEntry function"]
ms.keywords: FsRtlAddMcbEntry, FsRtlAddMcbEntry function [Installable File System Drivers], fsrtlref_73de29f7-837c-40a4-b224-ab7266794840.xml, ifsk.fsrtladdmcbentry, ntifs/FsRtlAddMcbEntry
req.header: ntifs.h
req.include-header: Ntifs.h
req.target-type: Windows
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
ms.custom: RS5
f1_keywords:
 - FsRtlAddMcbEntry
 - ntifs/FsRtlAddMcbEntry
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - ntifs.h
api_name:
 - FsRtlAddMcbEntry
dev_langs:
 - c++
---

# FsRtlAddMcbEntry function


## -description

The <b>FsRtlAddMcbEntry</b> routine is obsolete, but is exported to support existing driver binaries. Use <a href="/windows-hardware/drivers/ddi/ntifs/nf-ntifs-_fsrtl_advanced_fcb_header-fsrtladdlargemcbentry">FsRtlAddLargeMcbEntry</a> instead.

## -parameters

### -param Mcb

<p>Reserved.</p>

### -param Vbn

Reserved.

### -param Lbn

Reserved.

### -param SectorCount

Reserved.
