---
UID: NS:rilapitypes.RILMESSAGE
title: RILMESSAGE
author: windows-driver-content
description: This topic supports the Windows driver infrastructure and is not intended to be used directly from your code.
old-location: netvista\rilmessage_2.htm
old-project: netvista
ms.assetid: 731ae115-2394-4651-9b79-6d640d07a328
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: "*LPRILMESSAGE, RILMESSAGE, RILMESSAGE structure [Network Drivers Starting with Windows Vista], netvista.rilmessage_2, rilapitypes/RILMESSAGE"
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
-	RILMESSAGE
product: Windows
targetos: Windows
req.typenames: RILMESSAGE, *LPRILMESSAGE
req.product: Windows 10 or later.
---

# RILMESSAGE structure


## -description


This topic supports the Windows driver infrastructure and is not intended to be used directly from your code. 


## -syntax


````
typedef struct _RILMESSAGE {
  DWORD                cbSize;
  DWORD                dwParams;
  RILADDRESS           raSvcCtrAddress;
  RILMESSAGETYPE       dwType;
  DWORD                dwFlags;
  NULL                 RILMSGUNION;
  RILMSGUNION          msgUnion;
  NULL                 switch_is;
  NULL                 dwType;
  RILMSGINDELIVER      unMsgInDeliver;
  NULL                 case;
  NULL                 RIL_MSGTYPE_IN_DELIVER;
  RILMSGINSTATUS       unMsgInStatus;
  NULL                 case;
  NULL                 RIL_MSGTYPE_IN_STATUS;
  RILMSGOUTSUBMIT      unMsgOutSubmit;
  NULL                 case;
  NULL                 RIL_MSGTYPE_OUT_SUBMIT;
  RILMSGBCGENERAL      unMsgBcGeneral;
  NULL                 case;
  NULL                 RIL_MSGTYPE_BC_GENERAL;
  RILMSGIS637INSTATUS  unMsgIS637InStatus;
  NULL                 case;
  NULL                 RIL_MSGTYPE_IN_IS637STATUS;
  RILMSGCDMAINDELIVER  unMsgCDMAInDeliver;
  NULL                 case;
  NULL                 RIL_MSGTYPE_IN_CDMADELIVER;
  RILMSGCDMAOUTSUBMIT  unMsgCDMAOutSubmit;
  NULL                 case;
  NULL                 RIL_MSGTYPE_OUT_CDMASUBMIT;
} RILMESSAGE, RILMESSAGE;
````


## -struct-fields




### -field cbSize


### -field dwParams


### -field raSvcCtrAddress


### -field dwType


### -field dwFlags


### -field msgUnion


### -field RILMSGUNION


#### - switch_is


#### - unMsgInDeliver


#### - case


#### - RIL_MSGTYPE_IN_DELIVER


#### - unMsgInStatus


#### - RIL_MSGTYPE_IN_STATUS


#### - unMsgOutSubmit


#### - RIL_MSGTYPE_OUT_SUBMIT


#### - unMsgBcGeneral


#### - RIL_MSGTYPE_BC_GENERAL


#### - unMsgIS637InStatus


#### - RIL_MSGTYPE_IN_IS637STATUS


#### - unMsgCDMAInDeliver


#### - RIL_MSGTYPE_IN_CDMADELIVER


#### - unMsgCDMAOutSubmit


#### - RIL_MSGTYPE_OUT_CDMASUBMIT
