---
UID: NF:ucxclass.UcxInitializeDeviceInit
title: UcxInitializeDeviceInit function (ucxclass.h)
description: UcxInitializeDeviceInit initializes device initialization operations when the Plug and Play (PnP) manager reports the existence of a device.
old-location: buses\_ucxinitializedeviceinit.htm
tech.root: usbref
ms.date: 05/07/2018
keywords: ["UcxInitializeDeviceInit function"]
ms.keywords: UcxInitializeDeviceInit, UcxInitializeDeviceInit method [Buses], buses._ucxinitializedeviceinit, ucxclass/UcxInitializeDeviceInit
req.header: ucxclass.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 10
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
targetos: Windows
req.typenames: 
f1_keywords:
 - UcxInitializeDeviceInit
 - ucxclass/UcxInitializeDeviceInit
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - ucxclass.h
api_name:
 - UcxInitializeDeviceInit
---

# UcxInitializeDeviceInit function


## -description

Initializes device initialization operations when the Plug and Play (PnP) manager reports the existence of a device.

## -parameters

### -param DeviceInit 

[in, out]
A pointer to a framework-allocated <a href="/windows-hardware/drivers/wdf/wdfdevice_init">WDFDEVICE_INIT</a> structure.

## -returns

(NTSTATUS) The method returns STATUS_SUCCESS if the operation succeeds. Otherwise, this method may return an appropriate <a href="/windows-hardware/drivers/kernel/ntstatus-values">NTSTATUS</a> error code.

## -remarks

The client driver for the host controller calls this method in its <a href="/windows-hardware/drivers/ddi/wdfdriver/nc-wdfdriver-evt_wdf_driver_device_add">EvtDriverDeviceAdd</a> implementation before it calls <a href="/windows-hardware/drivers/ddi/wdfdevice/nf-wdfdevice-wdfdevicecreate">WdfDeviceCreate</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/wdfdevice/nf-wdfdevice-wdfdevicecreate">WdfDeviceCreate</a>
