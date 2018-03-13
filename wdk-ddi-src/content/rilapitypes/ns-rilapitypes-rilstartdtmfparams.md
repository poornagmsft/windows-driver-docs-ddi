---
UID: NS:rilapitypes.RILSTARTDTMFPARAMS
title: RILSTARTDTMFPARAMS
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilstartdtmfparams_2.htm
old-project: netvista
ms.assetid: 51f6ea96-412a-429f-993b-de31f77f4d30
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: "*LPRILSTARTDTMFPARAMS, RILSTARTDTMFPARAMS, RILSTARTDTMFPARAMS structure [Network Drivers Starting with Windows Vista], netvista.rilstartdtmfparams_2, rilapitypes/RILSTARTDTMFPARAMS"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
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
req.lib: 
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
-	RILSTARTDTMFPARAMS
product: Windows
targetos: Windows
req.typenames: RILSTARTDTMFPARAMS, *LPRILSTARTDTMFPARAMS
req.product: Windows 10 or later.
---

# RILSTARTDTMFPARAMS structure


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef struct _RILSTARTDTMFPARAMS {
  DWORD  dwExecutor;
  char   ch;
} RILSTARTDTMFPARAMS, RILSTARTDTMFPARAMS;
````


## -struct-fields




### -field dwExecutor


### -field ch
