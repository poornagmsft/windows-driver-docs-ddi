---
UID: NE:rilapitypes.RILSERVICESETTINGSSTATUS
title: RILSERVICESETTINGSSTATUS
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilservicesettingsstatus_2.htm
old-project: netvista
ms.assetid: 4d193398-752f-4aef-8ae6-59c9afabd79a
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILSERVICESETTINGSSTATUS, RILSERVICESETTINGSSTATUS enumeration [Network Drivers Starting with Windows Vista], RIL_SVCSTAT_DEFAULT, RIL_SVCSTAT_DISABLED, RIL_SVCSTAT_ENABLED, RIL_SVCSTAT_MAX, netvista.rilservicesettingsstatus_2, rilapitypes/RILSERVICESETTINGSSTATUS, rilapitypes/RIL_SVCSTAT_DEFAULT, rilapitypes/RIL_SVCSTAT_DISABLED, rilapitypes/RIL_SVCSTAT_ENABLED, rilapitypes/RIL_SVCSTAT_MAX
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
-	RILSERVICESETTINGSSTATUS
product: Windows
targetos: Windows
req.typenames: RILSERVICESETTINGSSTATUS
req.product: Windows 10 or later.
---

# RILSERVICESETTINGSSTATUS enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILSERVICESETTINGSSTATUS { 
  RIL_SVCSTAT_DISABLED,
  RIL_SVCSTAT_ENABLED,
  RIL_SVCSTAT_DEFAULT,
  RIL_SVCSTAT_MAX
} RILSERVICESETTINGSSTATUS;
````


## -enum-fields




### -field RIL_SVCSTAT_UNKNOWN


### -field RIL_SVCSTAT_DISABLED


### -field RIL_SVCSTAT_ENABLED


### -field RIL_SVCSTAT_DEFAULT


### -field RIL_SVCSTAT_MAX
