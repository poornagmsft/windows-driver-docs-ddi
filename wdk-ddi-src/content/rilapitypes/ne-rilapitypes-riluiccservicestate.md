---
UID: NE:rilapitypes.RILUICCSERVICESTATE
title: RILUICCSERVICESTATE
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\riluiccservicestate_2.htm
old-project: netvista
ms.assetid: f817db6b-bda4-45cd-953b-fd3d81bafa8f
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILUICCSERVICESTATE, RILUICCSERVICESTATE enumeration [Network Drivers Starting with Windows Vista], RIL_UICCSERVICESTATE_DISABLED, RIL_UICCSERVICESTATE_ENABLED, RIL_UICCSERVICESTATE_MAX, netvista.riluiccservicestate_2, rilapitypes/RILUICCSERVICESTATE, rilapitypes/RIL_UICCSERVICESTATE_DISABLED, rilapitypes/RIL_UICCSERVICESTATE_ENABLED, rilapitypes/RIL_UICCSERVICESTATE_MAX
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
-	RILUICCSERVICESTATE
product: Windows
targetos: Windows
req.typenames: RILUICCSERVICESTATE
req.product: Windows 10 or later.
---

# RILUICCSERVICESTATE enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILUICCSERVICESTATE { 
  RIL_UICCSERVICESTATE_DISABLED,
  RIL_UICCSERVICESTATE_ENABLED,
  RIL_UICCSERVICESTATE_MAX
} RILUICCSERVICESTATE;
````


## -enum-fields




### -field RIL_UICCSERVICESTATE_NOTAVAILABLE


### -field RIL_UICCSERVICESTATE_DISABLED


### -field RIL_UICCSERVICESTATE_ENABLED


### -field RIL_UICCSERVICESTATE_MAX
