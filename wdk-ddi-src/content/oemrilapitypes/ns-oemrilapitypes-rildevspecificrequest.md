---
UID: NS:oemrilapitypes.RILDEVSPECIFICREQUEST
title: RILDEVSPECIFICREQUEST
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rildevspecificrequest.htm
old-project: netvista
ms.assetid: 36e2ae4b-cc2f-4980-95fe-25a38a1c07b1
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: "*LPRILDEVSPECIFICREQUEST, LPRILDEVSPECIFICREQUEST, LPRILDEVSPECIFICREQUEST structure pointer [Network Drivers Starting with Windows Vista], RILDEVSPECIFICREQUEST, RILDEVSPECIFICREQUEST structure [Network Drivers Starting with Windows Vista], netvista.rildevspecificrequest, oemrilapitypes/LPRILDEVSPECIFICREQUEST, oemrilapitypes/RILDEVSPECIFICREQUEST"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: oemrilapitypes.h
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
req.irql: PASSIVE_LEVEL
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	oemrilapitypes.h
api_name:
-	RILDEVSPECIFICREQUEST
product: Windows
targetos: Windows
req.typenames: RILDEVSPECIFICREQUEST, *LPRILDEVSPECIFICREQUEST
---

# RILDEVSPECIFICREQUEST structure


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.


## -syntax


````
typedef struct _RILDEVSPECIFICREQUEST {
  DWORD   dwCmdId;
  DWORD   dwSize;
  BYTE [] params;
} RILDEVSPECIFICREQUEST, *LPRILDEVSPECIFICREQUEST;
````


## -struct-fields




### -field dwCmdId


### -field dwSize


### -field params
