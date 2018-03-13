---
UID: NE:rilapitypes.RILSETSYSTEMSELECTIONPREFSFLAG
title: RILSETSYSTEMSELECTIONPREFSFLAG
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilsetsystemselectionprefsflag_2.htm
old-project: netvista
ms.assetid: d932f5c8-d6a6-4611-b6f2-12c501df1117
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILSETSYSTEMSELECTIONPREFSFLAG, RILSETSYSTEMSELECTIONPREFSFLAG enumeration [Network Drivers Starting with Windows Vista], RIL_SSSPFLAG_ALL, RIL_SSSPFLAG_APPLYIMMEDIATELY, RIL_SSSPFLAG_ENFORCESCAN, netvista.rilsetsystemselectionprefsflag_2, rilapitypes/RILSETSYSTEMSELECTIONPREFSFLAG, rilapitypes/RIL_SSSPFLAG_ALL, rilapitypes/RIL_SSSPFLAG_APPLYIMMEDIATELY, rilapitypes/RIL_SSSPFLAG_ENFORCESCAN
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: rilapitypes.h
req.include-header: 
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
req.lib: NtosKrnl.exe
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	rilapitypes.h
api_name:
-	RILSETSYSTEMSELECTIONPREFSFLAG
product: Windows
targetos: Windows
req.typenames: RILSETSYSTEMSELECTIONPREFSFLAG
req.product: Windows 10 or later.
---

# RILSETSYSTEMSELECTIONPREFSFLAG enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILSETSYSTEMSELECTIONPREFSFLAG { 
  RIL_SSSPFLAG_APPLYIMMEDIATELY,
  RIL_SSSPFLAG_ENFORCESCAN,
  RIL_SSSPFLAG_ALL
} RILSETSYSTEMSELECTIONPREFSFLAG;
````


## -enum-fields




### -field RIL_SSSPFLAG_NONE


### -field RIL_SSSPFLAG_APPLYIMMEDIATELY


### -field RIL_SSSPFLAG_ENFORCESCAN


### -field RIL_SSSPFLAG_ALL
