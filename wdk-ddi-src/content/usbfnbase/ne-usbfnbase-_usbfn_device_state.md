---
UID: NE:usbfnbase._USBFN_DEVICE_STATE
title: "_USBFN_DEVICE_STATE"
author: windows-driver-content
description: Defines the Universal Serial Bus (USB) device states for the device/controller. These states correspond to the USB device states as defined in section 9.1 of the USB 2.0 Specification.
old-location: buses\usbfn_device_state.htm
old-project: usbref
ms.assetid: B367D0F7-5026-4C88-B88A-69068F76B675
ms.author: windowsdriverdev
ms.date: 2/24/2018
ms.keywords: "*PUSBFN_DEVICE_STATE, USBFN_DEVICE_STATE, USBFN_DEVICE_STATE enumeration [Buses], UsbfnDeviceStateAddressed, UsbfnDeviceStateAttached, UsbfnDeviceStateConfigured, UsbfnDeviceStateDefault, UsbfnDeviceStateDetached, UsbfnDeviceStateMinimum, UsbfnDeviceStateStateMaximum, UsbfnDeviceStateSuspended, _USBFN_DEVICE_STATE, buses.usbfn_device_state, usbfnbase/USBFN_DEVICE_STATE, usbfnbase/UsbfnDeviceStateAddressed, usbfnbase/UsbfnDeviceStateAttached, usbfnbase/UsbfnDeviceStateConfigured, usbfnbase/UsbfnDeviceStateDefault, usbfnbase/UsbfnDeviceStateDetached, usbfnbase/UsbfnDeviceStateMinimum, usbfnbase/UsbfnDeviceStateStateMaximum, usbfnbase/UsbfnDeviceStateSuspended"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: usbfnbase.h
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
-	usbfnbase.h
api_name:
-	USBFN_DEVICE_STATE
product: Windows
targetos: Windows
req.typenames: USBFN_DEVICE_STATE, *PUSBFN_DEVICE_STATE
req.product: Windows 10 or later.
---

# _USBFN_DEVICE_STATE enumeration


## -description


Defines the Universal Serial Bus (USB) device states for the device/controller.  These states correspond to the USB device states as defined in section 9.1 of the USB 2.0 Specification.


## -syntax


````
typedef enum _USBFN_DEVICE_STATE { 
  UsbfnDeviceStateMinimum       = 0x0,
  UsbfnDeviceStateAttached,
  UsbfnDeviceStateDefault,
  UsbfnDeviceStateDetached,
  UsbfnDeviceStateAddressed,
  UsbfnDeviceStateConfigured,
  UsbfnDeviceStateSuspended,
  UsbfnDeviceStateStateMaximum
} USBFN_DEVICE_STATE;
````


## -enum-fields




### -field UsbfnDeviceStateMinimum

The minimum value of the enumeration.


### -field UsbfnDeviceStateAttached

Device is attached to an upstream port.


### -field UsbfnDeviceStateDefault

Device is attached and connected to an upstream port but has not been reset.


### -field UsbfnDeviceStateDetached

Device is not attached to an upstream port.


### -field UsbfnDeviceStateAddressed

Device has been assigned a non-default USB address by the host.


### -field UsbfnDeviceStateConfigured

Device has been configured by the host.


### -field UsbfnDeviceStateSuspended

Device has been suspended.


### -field UsbfnDeviceStateStateMaximum

The maximum value of the enumeration.
