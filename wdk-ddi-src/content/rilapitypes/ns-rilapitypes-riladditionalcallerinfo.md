---
UID: NS:rilapitypes.RILADDITIONALCALLERINFO
title: RILADDITIONALCALLERINFO
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\riladditionalcallerinfo_2.htm
old-project: netvista
ms.assetid: e29f6710-0ca1-4420-b0e7-957ba020254b
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: "*LPRILADDITIONALCALLERINFO, RILADDITIONALCALLERINFO, RILADDITIONALCALLERINFO structure [Network Drivers Starting with Windows Vista], netvista.riladditionalcallerinfo_2, rilapitypes/RILADDITIONALCALLERINFO"
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
-	RILADDITIONALCALLERINFO
product: Windows
targetos: Windows
req.typenames: RILADDITIONALCALLERINFO, *LPRILADDITIONALCALLERINFO
req.product: Windows 10 or later.
---

# RILADDITIONALCALLERINFO structure


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef struct _RILADDITIONALCALLERINFO {
  DWORD     cbSize;
  DWORD     dwParams;
  DWORD     dwExecutor;
  DWORD     dwCallId;
  DWORD     dwCallerInfoLength;
  WCHAR [1] wszCallerInfo;
} RILADDITIONALCALLERINFO, RILADDITIONALCALLERINFO;
````


## -struct-fields




### -field cbSize


### -field dwParams


### -field dwExecutor


### -field dwCallId


### -field dwCallerInfoLength


### -field wszCallerInfo
