---
UID: NS:rilapitypes.RILPHONEBOOKLOCATION
title: RILPHONEBOOKLOCATION
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilphonebooklocation_2.htm
old-project: netvista
ms.assetid: 1878109a-f70c-4e4b-8735-7fbb972f4416
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: "*LPRILPHONEBOOKLOCATION, RILPHONEBOOKLOCATION, RILPHONEBOOKLOCATION structure [Network Drivers Starting with Windows Vista], netvista.rilphonebooklocation_2, rilapitypes/RILPHONEBOOKLOCATION"
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
-	RILPHONEBOOKLOCATION
product: Windows
targetos: Windows
req.typenames: RILPHONEBOOKLOCATION, *LPRILPHONEBOOKLOCATION
req.product: Windows 10 or later.
---

# RILPHONEBOOKLOCATION structure


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef struct _RILPHONEBOOKLOCATION {
  DWORD                       cbSize;
  HUICCAPP                    hUiccApp;
  RILPHONEENTRYSTORELOCATION  dwStoreLocation;
  DWORD                       dwIndex;
} RILPHONEBOOKLOCATION, RILPHONEBOOKLOCATION;
````


## -struct-fields




### -field cbSize


### -field hUiccApp


### -field dwStoreLocation


### -field dwIndex
