---
UID: NE:rilapitypes.RILTONESIGNALINFOPARAMMASK
title: RILTONESIGNALINFOPARAMMASK
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\riltonesignalinfoparammask_2.htm
old-project: netvista
ms.assetid: 1eeca3ef-6e1d-486f-b700-5ab8718a9285
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILTONESIGNALINFOPARAMMASK, RILTONESIGNALINFOPARAMMASK enumeration [Network Drivers Starting with Windows Vista], RIL_PARAM_TONESIGNAL_All, RIL_PARAM_TONESIGNAL_EXECUTOR, RIL_PARAM_TONESIGNAL_GPP2ISDNALERTING, RIL_PARAM_TONESIGNAL_GPP2TONE, netvista.riltonesignalinfoparammask_2, rilapitypes/RILTONESIGNALINFOPARAMMASK, rilapitypes/RIL_PARAM_TONESIGNAL_All, rilapitypes/RIL_PARAM_TONESIGNAL_EXECUTOR, rilapitypes/RIL_PARAM_TONESIGNAL_GPP2ISDNALERTING, rilapitypes/RIL_PARAM_TONESIGNAL_GPP2TONE
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
-	RILTONESIGNALINFOPARAMMASK
product: Windows
targetos: Windows
req.typenames: RILTONESIGNALINFOPARAMMASK
req.product: Windows 10 or later.
---

# RILTONESIGNALINFOPARAMMASK enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILTONESIGNALINFOPARAMMASK { 
  RIL_PARAM_TONESIGNAL_GPP2TONE,
  RIL_PARAM_TONESIGNAL_GPP2ISDNALERTING,
  RIL_PARAM_TONESIGNAL_EXECUTOR,
  RIL_PARAM_TONESIGNAL_All
} RILTONESIGNALINFOPARAMMASK;
````


## -enum-fields




### -field RIL_PARAM_TONESIGNAL_GPPTONE


### -field RIL_PARAM_TONESIGNAL_GPP2TONE


### -field RIL_PARAM_TONESIGNAL_GPP2ISDNALERTING


### -field RIL_PARAM_TONESIGNAL_EXECUTOR


### -field RIL_PARAM_TONESIGNAL_All
