---
UID: NS:ntddrilapitypes.RILEXCHANGEUICCAPDURESPONSE
title: RILEXCHANGEUICCAPDURESPONSE
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilexchangeuiccapduresponse.htm
old-project: netvista
ms.assetid: 57418ab1-e341-41ad-a120-cc4f7e0b0227
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: "*LPRILEXCHANGEUICCAPDURESPONSE, RILEXCHANGEUICCAPDURESPONSE, RILEXCHANGEUICCAPDURESPONSE structure [Network Drivers Starting with Windows Vista], netvista.rilexchangeuiccapduresponse, ntddrilapitypes/RILEXCHANGEUICCAPDURESPONSE"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ntddrilapitypes.h
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
-	ntddrilapitypes.h
api_name:
-	RILEXCHANGEUICCAPDURESPONSE
product: Windows
targetos: Windows
req.typenames: RILEXCHANGEUICCAPDURESPONSE, *LPRILEXCHANGEUICCAPDURESPONSE
---

# RILEXCHANGEUICCAPDURESPONSE structure


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.


## -syntax


````
typedef struct _RILEXCHANGEUICCAPDURESPONSE {
  DWORD    cbSize;
  DWORD    dwParams;
  DWORD    dwResponseAPDULength;
  BYTE [1] bResponseAPDU;
} RILEXCHANGEUICCAPDURESPONSE, RILEXCHANGEUICCAPDURESPONSE;
````


## -struct-fields




### -field cbSize


### -field dwParams


### -field dwResponseAPDULength


### -field bResponseAPDU
