---
UID: NF:storport.ScsiPortReadRegisterUchar
title: ScsiPortReadRegisterUchar macro (storport.h)
description: Learn how the ScsiPortReadRegisterUchar routine reads an unsigned byte value from the HBA.Note  The SCSI port driver and SCSI miniport driver models may be altered or unavailable in the future.
old-location: storage\scsiportreadregisteruchar.htm
tech.root: storage
ms.date: 03/29/2018
keywords: ["ScsiPortReadRegisterUchar macro"]
ms.keywords: ScsiPortReadRegisterUchar, ScsiPortReadRegisterUchar routine [Storage Devices], scsiprt_220f8972-dc09-4027-9cec-85a07ed5547d.xml, srb/ScsiPortReadRegisterUchar, storage.scsiportreadregisteruchar
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
 - ScsiPortReadRegisterUchar
 - storport/ScsiPortReadRegisterUchar
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - LibDef
api_location:
 - Scsiport.lib
 - Scsiport.dll
api_name:
 - ScsiPortReadRegisterUchar
---

# ScsiPortReadRegisterUchar macro


## -description

The <b>ScsiPortReadRegisterUchar</b> routine reads an unsigned byte value from the HBA.
<div class="alert"><b>Note</b>  The SCSI port driver and SCSI miniport driver models may be altered or unavailable in the future. Instead, we recommend using the <a href="/windows-hardware/drivers/storage/storport-driver">Storport driver</a> and <a href="/windows-hardware/drivers/storage/storport-miniport-drivers">Storport miniport</a> driver models.</div><div> </div>

## -parameters

### -param Register 

[in]
Pointer to the register. The given <i>Register</i> must be in a mapped memory-space range returned by <b>ScsiPortGetDeviceBase</b>.

## -remarks

<b>ScsiPortReadRegisterUchar</b> ensures that the data is transferred correctly.

## -see-also

<a href="/windows-hardware/drivers/ddi/srb/nf-srb-scsiportgetdevicebase">ScsiPortGetDeviceBase</a>
