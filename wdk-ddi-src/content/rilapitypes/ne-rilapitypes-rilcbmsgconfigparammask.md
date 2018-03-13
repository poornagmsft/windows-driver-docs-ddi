---
UID: NE:rilapitypes.RILCBMSGCONFIGPARAMMASK
title: RILCBMSGCONFIGPARAMMASK
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilcbmsgconfigparammask_2.htm
old-project: netvista
ms.assetid: ec2a26a0-4325-41d9-a6b4-5b9c2f22dd4e
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILCBMSGCONFIGPARAMMASK, RILCBMSGCONFIGPARAMMASK enumeration [Network Drivers Starting with Windows Vista], RIL_PARAM_CBMC_ALL, RIL_PARAM_CBMC_CDMAINFO, RIL_PARAM_CBMC_CDMASIZE, RIL_PARAM_CBMC_GWLINFO, netvista.rilcbmsgconfigparammask_2, rilapitypes/RILCBMSGCONFIGPARAMMASK, rilapitypes/RIL_PARAM_CBMC_ALL, rilapitypes/RIL_PARAM_CBMC_CDMAINFO, rilapitypes/RIL_PARAM_CBMC_CDMASIZE, rilapitypes/RIL_PARAM_CBMC_GWLINFO
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
-	RILCBMSGCONFIGPARAMMASK
product: Windows
targetos: Windows
req.typenames: RILCBMSGCONFIGPARAMMASK
req.product: Windows 10 or later.
---

# RILCBMSGCONFIGPARAMMASK enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILCBMSGCONFIGPARAMMASK { 
  RIL_PARAM_CBMC_GWLINFO,
  RIL_PARAM_CBMC_CDMASIZE,
  RIL_PARAM_CBMC_CDMAINFO,
  RIL_PARAM_CBMC_ALL
} RILCBMSGCONFIGPARAMMASK;
````


## -enum-fields




### -field RIL_PARAM_CBMC_GWLSIZE


### -field RIL_PARAM_CBMC_GWLINFO


### -field RIL_PARAM_CBMC_CDMASIZE


### -field RIL_PARAM_CBMC_CDMAINFO


### -field RIL_PARAM_CBMC_ALL
