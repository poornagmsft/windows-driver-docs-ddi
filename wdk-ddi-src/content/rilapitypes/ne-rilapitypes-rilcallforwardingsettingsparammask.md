---
UID: NE:rilapitypes.RILCALLFORWARDINGSETTINGSPARAMMASK
title: RILCALLFORWARDINGSETTINGSPARAMMASK
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilcallforwardingsettingsparammask_2.htm
old-project: netvista
ms.assetid: 4db4e6fe-1faf-4109-95aa-e2e5bf3b0dd6
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILCALLFORWARDINGSETTINGSPARAMMASK, RILCALLFORWARDINGSETTINGSPARAMMASK enumeration [Network Drivers Starting with Windows Vista], RIL_PARAM_CFS_ADDRESS, RIL_PARAM_CFS_ALL, RIL_PARAM_CFS_DELAYTIME, RIL_PARAM_CFS_INFOCLASSES, RIL_PARAM_CFS_SUBADDRESS, netvista.rilcallforwardingsettingsparammask_2, rilapitypes/RILCALLFORWARDINGSETTINGSPARAMMASK, rilapitypes/RIL_PARAM_CFS_ADDRESS, rilapitypes/RIL_PARAM_CFS_ALL, rilapitypes/RIL_PARAM_CFS_DELAYTIME, rilapitypes/RIL_PARAM_CFS_INFOCLASSES, rilapitypes/RIL_PARAM_CFS_SUBADDRESS
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
-	RILCALLFORWARDINGSETTINGSPARAMMASK
product: Windows
targetos: Windows
req.typenames: RILCALLFORWARDINGSETTINGSPARAMMASK
req.product: Windows 10 or later.
---

# RILCALLFORWARDINGSETTINGSPARAMMASK enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILCALLFORWARDINGSETTINGSPARAMMASK { 
  RIL_PARAM_CFS_INFOCLASSES,
  RIL_PARAM_CFS_ADDRESS,
  RIL_PARAM_CFS_SUBADDRESS,
  RIL_PARAM_CFS_DELAYTIME,
  RIL_PARAM_CFS_ALL
} RILCALLFORWARDINGSETTINGSPARAMMASK;
````


## -enum-fields




### -field RIL_PARAM_CFS_STATUS


### -field RIL_PARAM_CFS_INFOCLASSES


### -field RIL_PARAM_CFS_ADDRESS


### -field RIL_PARAM_CFS_SUBADDRESS


### -field RIL_PARAM_CFS_DELAYTIME


### -field RIL_PARAM_CFS_ALL
