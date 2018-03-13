---
UID: NE:rilapitypes.RILGEOLOCATIONTYPEMASK
title: RILGEOLOCATIONTYPEMASK
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilgeolocationtypemask_2.htm
old-project: netvista
ms.assetid: ffbd2c6d-537a-44f7-a071-21c073d96264
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILGEOLOCATIONTYPEMASK, RILGEOLOCATIONTYPEMASK enumeration [Network Drivers Starting with Windows Vista], RIL_GEOLOCATION_ALL, RIL_GEOLOCATION_CIVIC, RIL_GEOLOCATION_LATLONG, netvista.rilgeolocationtypemask_2, rilapitypes/RILGEOLOCATIONTYPEMASK, rilapitypes/RIL_GEOLOCATION_ALL, rilapitypes/RIL_GEOLOCATION_CIVIC, rilapitypes/RIL_GEOLOCATION_LATLONG
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
-	RILGEOLOCATIONTYPEMASK
product: Windows
targetos: Windows
req.typenames: RILGEOLOCATIONTYPEMASK
req.product: Windows 10 or later.
---

# RILGEOLOCATIONTYPEMASK enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILGEOLOCATIONTYPEMASK { 
  RIL_GEOLOCATION_CIVIC,
  RIL_GEOLOCATION_LATLONG,
  RIL_GEOLOCATION_ALL
} RILGEOLOCATIONTYPEMASK;
````


## -enum-fields




### -field RIL_GEOLOCATION_NONE


### -field RIL_GEOLOCATION_CIVIC


### -field RIL_GEOLOCATION_LATLONG


### -field RIL_GEOLOCATION_ALL
