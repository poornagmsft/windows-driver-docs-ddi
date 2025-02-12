---
UID: NC:d3dkmthk.PFND3DKMT_OFFERALLOCATIONS
title: PFND3DKMT_OFFERALLOCATIONS (d3dkmthk.h)
description: The PFND3DKMT_OFFERALLOCATIONS callback offers video memory allocations for reuse. The function returns STATUS_SUCCESS if allocations were successfully offered.
old-location: display\d3dkmtofferallocations.htm
ms.date: 05/10/2018
keywords: ["PFND3DKMT_OFFERALLOCATIONS callback function"]
ms.keywords: D3DKMTOfferAllocations, D3DKMTOfferAllocations callback function [Display Devices], PFND3DKMT_OFFERALLOCATIONS, PFND3DKMT_OFFERALLOCATIONS callback, d3dkmthk/D3DKMTOfferAllocations, display.d3dkmtofferallocations
req.header: d3dkmthk.h
req.include-header: D3dkmthk.h
req.target-type: Universal
req.target-min-winverclnt: Windows 8
req.target-min-winversvr: Windows Server 2012
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
targetos: Windows
tech.root: display
req.typenames: 
f1_keywords:
 - PFND3DKMT_OFFERALLOCATIONS
 - d3dkmthk/PFND3DKMT_OFFERALLOCATIONS
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - D3dkmthk.h
api_name:
 - PFND3DKMT_OFFERALLOCATIONS
---

# PFND3DKMT_OFFERALLOCATIONS callback function


## -description

Offers video memory allocations for reuse.

## -parameters

### -param unnamedParam1

*pData* 

[in] A pointer to a <a href="/windows-hardware/drivers/ddi/d3dkmthk/ns-d3dkmthk-_d3dkmt_offerallocations">D3DKMT_OFFERALLOCATIONS</a> structure that defines memory allocations that the driver offers for reuse.

## -returns

Returns one of the following values:

|Return code|Description|
|--- |--- |
|STATUS_SUCCESS|The allocations were successfully offered.|
|STATUS_DEVICE_REMOVED|The graphics adapter was stopped or the display device was reset.|
|STATUS_INVALID_PARAMETER|Parameters were validated and determined to be incorrect.|

## -see-also

<a href="/windows-hardware/drivers/ddi/d3dkmthk/nf-d3dkmthk-d3dkmtreclaimallocations">D3DKMTReclaimAllocations</a>



<a href="/windows-hardware/drivers/ddi/d3dkmthk/ns-d3dkmthk-_d3dkmt_offerallocations">D3DKMT_OFFERALLOCATIONS</a>

