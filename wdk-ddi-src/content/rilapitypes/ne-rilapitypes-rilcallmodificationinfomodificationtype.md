---
UID: NE:rilapitypes.RILCALLMODIFICATIONINFOMODIFICATIONTYPE
title: RILCALLMODIFICATIONINFOMODIFICATIONTYPE
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilcallmodificationinfomodificationtype_2.htm
old-project: netvista
ms.assetid: e73abe84-1688-40f1-9b8c-e4e34cc87b78
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILCALLMODIFICATIONINFOMODIFICATIONTYPE, RILCALLMODIFICATIONINFOMODIFICATIONTYPE enumeration [Network Drivers Starting with Windows Vista], RIL_CALLMODIFICATIONTYPE_BLOCKED, RIL_CALLMODIFICATIONTYPE_MAX, RIL_CALLMODIFICATIONTYPE_MODIFIED, netvista.rilcallmodificationinfomodificationtype_2, rilapitypes/RILCALLMODIFICATIONINFOMODIFICATIONTYPE, rilapitypes/RIL_CALLMODIFICATIONTYPE_BLOCKED, rilapitypes/RIL_CALLMODIFICATIONTYPE_MAX, rilapitypes/RIL_CALLMODIFICATIONTYPE_MODIFIED
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
-	RILCALLMODIFICATIONINFOMODIFICATIONTYPE
product: Windows
targetos: Windows
req.typenames: RILCALLMODIFICATIONINFOMODIFICATIONTYPE
req.product: Windows 10 or later.
---

# RILCALLMODIFICATIONINFOMODIFICATIONTYPE enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILCALLMODIFICATIONINFOMODIFICATIONTYPE { 
  RIL_CALLMODIFICATIONTYPE_BLOCKED,
  RIL_CALLMODIFICATIONTYPE_MODIFIED,
  RIL_CALLMODIFICATIONTYPE_MAX
} RILCALLMODIFICATIONINFOMODIFICATIONTYPE;
````


## -enum-fields




### -field RIL_CALLMODIFICATIONTYPE_UNKNOWN


### -field RIL_CALLMODIFICATIONTYPE_BLOCKED


### -field RIL_CALLMODIFICATIONTYPE_MODIFIED


### -field RIL_CALLMODIFICATIONTYPE_MAX
