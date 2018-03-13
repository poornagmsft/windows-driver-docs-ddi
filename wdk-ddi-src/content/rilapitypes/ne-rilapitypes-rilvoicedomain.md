---
UID: NE:rilapitypes.RILVOICEDOMAIN
title: RILVOICEDOMAIN
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilvoicedomain_2.htm
old-project: netvista
ms.assetid: bc0e9ba8-c790-402a-900a-7ae2b4f76060
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILVOICEDOMAIN, RILVOICEDOMAIN enumeration [Network Drivers Starting with Windows Vista], RIL_VOICE_DOMAIN_3GPP, RIL_VOICE_DOMAIN_3GPP2, RIL_VOICE_DOMAIN_IMS, RIL_VOICE_DOMAIN_MAX, netvista.rilvoicedomain_2, rilapitypes/RILVOICEDOMAIN, rilapitypes/RIL_VOICE_DOMAIN_3GPP, rilapitypes/RIL_VOICE_DOMAIN_3GPP2, rilapitypes/RIL_VOICE_DOMAIN_IMS, rilapitypes/RIL_VOICE_DOMAIN_MAX
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
-	RILVOICEDOMAIN
product: Windows
targetos: Windows
req.typenames: RILVOICEDOMAIN
req.product: Windows 10 or later.
---

# RILVOICEDOMAIN enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILVOICEDOMAIN { 
  RIL_VOICE_DOMAIN_3GPP,
  RIL_VOICE_DOMAIN_3GPP2,
  RIL_VOICE_DOMAIN_IMS,
  RIL_VOICE_DOMAIN_MAX
} RILVOICEDOMAIN;
````


## -enum-fields




### -field RIL_VOICE_DOMAIN_NONE


### -field RIL_VOICE_DOMAIN_3GPP


### -field RIL_VOICE_DOMAIN_3GPP2


### -field RIL_VOICE_DOMAIN_IMS


### -field RIL_VOICE_DOMAIN_MAX
