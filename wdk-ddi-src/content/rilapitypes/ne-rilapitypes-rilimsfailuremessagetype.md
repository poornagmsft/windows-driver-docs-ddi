---
UID: NE:rilapitypes.RILIMSFAILUREMESSAGETYPE
title: RILIMSFAILUREMESSAGETYPE
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilimsfailuremessagetype_2.htm
old-project: netvista
ms.assetid: 9a29cc8c-7e46-4b7f-a428-d2f174945654
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILIMSFAILUREMESSAGETYPE, RILIMSFAILUREMESSAGETYPE enumeration [Network Drivers Starting with Windows Vista], RIL_IMSFAILUREMESSAGETYPE_INCALL, RIL_IMSFAILUREMESSAGETYPE_MAX, RIL_IMSFAILUREMESSAGETYPE_SUBSCRIBE, netvista.rilimsfailuremessagetype_2, rilapitypes/RILIMSFAILUREMESSAGETYPE, rilapitypes/RIL_IMSFAILUREMESSAGETYPE_INCALL, rilapitypes/RIL_IMSFAILUREMESSAGETYPE_MAX, rilapitypes/RIL_IMSFAILUREMESSAGETYPE_SUBSCRIBE
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
-	RILIMSFAILUREMESSAGETYPE
product: Windows
targetos: Windows
req.typenames: RILIMSFAILUREMESSAGETYPE
req.product: Windows 10 or later.
---

# RILIMSFAILUREMESSAGETYPE enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILIMSFAILUREMESSAGETYPE { 
  RIL_IMSFAILUREMESSAGETYPE_SUBSCRIBE,
  RIL_IMSFAILUREMESSAGETYPE_INCALL,
  RIL_IMSFAILUREMESSAGETYPE_MAX
} RILIMSFAILUREMESSAGETYPE;
````


## -enum-fields




### -field RIL_IMSFAILUREMESSAGETYPE_REGISTER


### -field RIL_IMSFAILUREMESSAGETYPE_SUBSCRIBE


### -field RIL_IMSFAILUREMESSAGETYPE_INCALL


### -field RIL_IMSFAILUREMESSAGETYPE_MAX
