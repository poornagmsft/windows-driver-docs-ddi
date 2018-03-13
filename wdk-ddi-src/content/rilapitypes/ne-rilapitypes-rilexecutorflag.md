---
UID: NE:rilapitypes.RILEXECUTORFLAG
title: RILEXECUTORFLAG
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilexecutorflag_2.htm
old-project: netvista
ms.assetid: 691d962a-5775-462a-8c3f-d9b02e189810
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: RILEXECUTORFLAG, RILEXECUTORFLAG enumeration [Network Drivers Starting with Windows Vista], RIL_EXECUTORFLAG_ALL, RIL_EXECUTORFLAG_HIGHPRIORITY, netvista.rilexecutorflag_2, rilapitypes/RILEXECUTORFLAG, rilapitypes/RIL_EXECUTORFLAG_ALL, rilapitypes/RIL_EXECUTORFLAG_HIGHPRIORITY
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
-	RILEXECUTORFLAG
product: Windows
targetos: Windows
req.typenames: RILEXECUTORFLAG
req.product: Windows 10 or later.
---

# RILEXECUTORFLAG enumeration


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef enum _RILEXECUTORFLAG { 
  RIL_EXECUTORFLAG_HIGHPRIORITY,
  RIL_EXECUTORFLAG_ALL
} RILEXECUTORFLAG;
````


## -enum-fields




### -field RIL_EXECUTORFLAG_ENABLED


### -field RIL_EXECUTORFLAG_HIGHPRIORITY


### -field RIL_EXECUTORFLAG_ALL
