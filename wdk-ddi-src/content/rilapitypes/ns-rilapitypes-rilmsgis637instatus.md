---
UID: NS:rilapitypes.RILMSGIS637INSTATUS
title: RILMSGIS637INSTATUS
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilmsgis637instatus_2.htm
old-project: netvista
ms.assetid: 70215db8-52c0-48c5-8e59-c60a61fbd07e
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: "*LPRILMSGIS637INSTATUS, RILMSGIS637INSTATUS, RILMSGIS637INSTATUS structure [Network Drivers Starting with Windows Vista], netvista.rilmsgis637instatus_2, rilapitypes/RILMSGIS637INSTATUS"
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
-	RILMSGIS637INSTATUS
product: Windows
targetos: Windows
req.typenames: RILMSGIS637INSTATUS, *LPRILMSGIS637INSTATUS
req.product: Windows 10 or later.
---

# RILMSGIS637INSTATUS structure


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef struct _RILMSGIS637INSTATUS {
  RILADDRESS               raOrigAddress;
  RILSUBADDRESS            rsaOrigSubaddr;
  RILSYSTEMTIME            stSCReceiveTime;
  DWORD                    dwCauseCode;
  DWORD                    dwReplySeqNumber;
  DWORD                    dwUserResponseCode;
  RILMSGCDMAMSGSTATUSTYPE  dwMsgStatusType;
  DWORD                    dwMsgID;
  RILMSGCDMALANGUAGE       dwMsgLang;
  RILMSGCDMAMSGENCODING    dwMsgEncoding;
  DWORD                    cchMsgLength;
  BYTE [MAXLENGTH_MSG]     rgbMsg;
} RILMSGIS637INSTATUS, RILMSGIS637INSTATUS;
````


## -struct-fields




### -field raOrigAddress


### -field rsaOrigSubaddr


### -field stSCReceiveTime


### -field dwCauseCode


### -field dwReplySeqNumber


### -field dwUserResponseCode


### -field dwMsgStatusType


### -field dwMsgID


### -field dwMsgLang


### -field dwMsgEncoding


### -field cchMsgLength


### -field rgbMsg
