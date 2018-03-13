---
UID: NE:rilapitypes.RILUICCAPPINFOPARAMMASK
title: RILUICCAPPINFOPARAMMASK
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\riluiccappinfoparammask_2.htm
old-project: netvista
ms.assetid: 17ca9b1c-aaf9-434e-be60-5698aa159b48
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILUICCAPPINFOPARAMMASK, RILUICCAPPINFOPARAMMASK enumeration [Network Drivers Starting with Windows Vista], RIL_PARAM_UICCAPPINFO_ALL, RIL_PARAM_UICCAPPINFO_APPID, RIL_PARAM_UICCAPPINFO_APPIDLENGTH, RIL_PARAM_UICCAPPINFO_APPNAME, RIL_PARAM_UICCAPPINFO_APPNAMELENGTH, RIL_PARAM_UICCAPPINFO_APPTYPE, RIL_PARAM_UICCAPPINFO_NUMPINS, RIL_PARAM_UICCAPPINFO_PINREF, netvista.riluiccappinfoparammask_2, rilapitypes/RILUICCAPPINFOPARAMMASK, rilapitypes/RIL_PARAM_UICCAPPINFO_ALL, rilapitypes/RIL_PARAM_UICCAPPINFO_APPID, rilapitypes/RIL_PARAM_UICCAPPINFO_APPIDLENGTH, rilapitypes/RIL_PARAM_UICCAPPINFO_APPNAME, rilapitypes/RIL_PARAM_UICCAPPINFO_APPNAMELENGTH, rilapitypes/RIL_PARAM_UICCAPPINFO_APPTYPE, rilapitypes/RIL_PARAM_UICCAPPINFO_NUMPINS, rilapitypes/RIL_PARAM_UICCAPPINFO_PINREF
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
-	RILUICCAPPINFOPARAMMASK
product: Windows
targetos: Windows
req.typenames: RILUICCAPPINFOPARAMMASK
req.product: Windows 10 or later.
---

# RILUICCAPPINFOPARAMMASK enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILUICCAPPINFOPARAMMASK { 
  RIL_PARAM_UICCAPPINFO_APPTYPE,
  RIL_PARAM_UICCAPPINFO_APPIDLENGTH,
  RIL_PARAM_UICCAPPINFO_APPID,
  RIL_PARAM_UICCAPPINFO_APPNAMELENGTH,
  RIL_PARAM_UICCAPPINFO_APPNAME,
  RIL_PARAM_UICCAPPINFO_NUMPINS,
  RIL_PARAM_UICCAPPINFO_PINREF,
  RIL_PARAM_UICCAPPINFO_ALL
} RILUICCAPPINFOPARAMMASK;
````


## -enum-fields




### -field RIL_PARAM_UICCAPPINFO_HUICCAPP


### -field RIL_PARAM_UICCAPPINFO_APPTYPE


### -field RIL_PARAM_UICCAPPINFO_APPIDLENGTH


### -field RIL_PARAM_UICCAPPINFO_APPID


### -field RIL_PARAM_UICCAPPINFO_APPNAMELENGTH


### -field RIL_PARAM_UICCAPPINFO_APPNAME


### -field RIL_PARAM_UICCAPPINFO_NUMPINS


### -field RIL_PARAM_UICCAPPINFO_PINREF


### -field RIL_PARAM_UICCAPPINFO_ALL
