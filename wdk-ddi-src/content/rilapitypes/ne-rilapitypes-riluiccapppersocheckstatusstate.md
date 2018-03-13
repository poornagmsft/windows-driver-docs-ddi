---
UID: NE:rilapitypes.RILUICCAPPPERSOCHECKSTATUSSTATE
title: RILUICCAPPPERSOCHECKSTATUSSTATE
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\riluiccapppersocheckstatusstate_2.htm
old-project: netvista
ms.assetid: 389c20de-7ff2-47c6-8393-529e401e56e0
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILUICCAPPPERSOCHECKSTATUSSTATE, RILUICCAPPPERSOCHECKSTATUSSTATE enumeration [Network Drivers Starting with Windows Vista], RIL_PERSOCHECKSTATE_FAIL, RIL_PERSOCHECKSTATE_MAX, RIL_PERSOCHECKSTATE_PASS, netvista.riluiccapppersocheckstatusstate_2, rilapitypes/RILUICCAPPPERSOCHECKSTATUSSTATE, rilapitypes/RIL_PERSOCHECKSTATE_FAIL, rilapitypes/RIL_PERSOCHECKSTATE_MAX, rilapitypes/RIL_PERSOCHECKSTATE_PASS
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
-	RILUICCAPPPERSOCHECKSTATUSSTATE
product: Windows
targetos: Windows
req.typenames: RILUICCAPPPERSOCHECKSTATUSSTATE
req.product: Windows 10 or later.
---

# RILUICCAPPPERSOCHECKSTATUSSTATE enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILUICCAPPPERSOCHECKSTATUSSTATE { 
  RIL_PERSOCHECKSTATE_PASS,
  RIL_PERSOCHECKSTATE_FAIL,
  RIL_PERSOCHECKSTATE_MAX
} RILUICCAPPPERSOCHECKSTATUSSTATE;
````


## -enum-fields




### -field RIL_PERSOCHECKSTATE_NOTREADY


### -field RIL_PERSOCHECKSTATE_PASS


### -field RIL_PERSOCHECKSTATE_FAIL


### -field RIL_PERSOCHECKSTATE_MAX
