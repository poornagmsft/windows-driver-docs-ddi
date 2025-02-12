---
UID: NF:storport.ScsiPortReadPortUlong
title: ScsiPortReadPortUlong macro (storport.h)
description: Learn how the ScsiPortReadPortUlong routine reads a ULONG value from the HBA.Note  The SCSI port driver and SCSI miniport driver models may be altered or unavailable in the future.
old-location: storage\scsiportreadportulong.htm
tech.root: storage
ms.date: 03/29/2018
keywords: ["ScsiPortReadPortUlong macro"]
ms.keywords: ScsiPortReadPortUlong, ScsiPortReadPortUlong routine [Storage Devices], scsiprt_af6cc9e1-eaa8-4c05-a695-ed54690d0f3b.xml, srb/ScsiPortReadPortUlong, storage.scsiportreadportulong
req.header: storport.h
req.include-header: Miniport.h, Scsi.h, Storport.h
req.target-type: Desktop
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
req.lib: Scsiport.lib
req.dll: 
req.irql: 
targetos: Windows
req.typenames: 
f1_keywords:
 - ScsiPortReadPortUlong
 - storport/ScsiPortReadPortUlong
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - Scsiport.lib
 - Scsiport.dll
api_name:
 - ScsiPortReadPortUlong
---

# ScsiPortReadPortUlong macro


## -description

The <b>ScsiPortReadPortUlong</b> routine reads a ULONG value from the HBA.
<div class="alert"><b>Note</b>  The SCSI port driver and SCSI miniport driver models may be altered or unavailable in the future. Instead, we recommend using the <a href="/windows-hardware/drivers/storage/storport-driver">Storport driver</a> and <a href="/windows-hardware/drivers/storage/storport-miniport-drivers">Storport miniport</a> driver models.</div><div> </div>

## -parameters

### -param Port 

[in]
Pointer to the I/O port. The given <i>Port</i> must be in a mapped I/O-space range returned by <b>ScsiPortGetDeviceBase</b>.

## -remarks

<b>ScsiPortReadPortUlong</b> ensures that the data is transferred correctly.

## -see-also

<a href="/windows-hardware/drivers/ddi/srb/nf-srb-scsiportgetdevicebase">ScsiPortGetDeviceBase</a>
