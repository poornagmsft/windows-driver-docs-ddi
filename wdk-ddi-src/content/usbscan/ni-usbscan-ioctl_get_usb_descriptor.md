---
UID: NI:usbscan.IOCTL_GET_USB_DESCRIPTOR
title: IOCTL_GET_USB_DESCRIPTOR
author: windows-driver-content
description: Returns a specified USB Descriptor.
old-location: image\ioctl_get_usb_descriptor.htm
old-project: image
ms.assetid: a5490a2a-d406-4029-b8be-446236a936bb
ms.author: windowsdriverdev
ms.date: 2/23/2018
ms.keywords: IOCTL_GET_USB_DESCRIPTOR, IOCTL_GET_USB_DESCRIPTOR control code [Imaging Devices], image.ioctl_get_usb_descriptor, stifnc_9d8ca100-d268-4e51-88fb-925e0a029ece.xml, usbscan/IOCTL_GET_USB_DESCRIPTOR
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: ioctl
req.header: usbscan.h
req.include-header: Usbscan.h
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
-	Usbscan.h
api_name:
-	IOCTL_GET_USB_DESCRIPTOR
product: Windows
targetos: Windows
req.typenames: RAW_PIPE_TYPE
req.product: Windows 10 or later.
---

# IOCTL_GET_USB_DESCRIPTOR IOCTL


##  Major Code: 


[IRP_MJ_DEVICE_CONTROL](https://docs.microsoft.com/en-us/windows-hardware/drivers/kernel/irp-mj-device-control)

## -description


Returns a specified USB Descriptor.


## -ioctlparameters




### -input-buffer

Pointer to a <a href="..\usbscan\ns-usbscan-_usbscan_get_descriptor.md">USBSCAN_GET_DESCRIPTOR</a> structure.


### -input-buffer-length

Size of the input buffer.


### -output-buffer

Pointer to a <a href="..\usbspec\ns-usbspec-_usb_device_descriptor.md">USB_DEVICE_DESCRIPTOR</a>, <a href="..\usbspec\ns-usbspec-_usb_string_descriptor.md">USB_STRING_DESCRIPTOR</a>, or <a href="..\usbspec\ns-usbspec-_usb_configuration_descriptor.md">USB_CONFIGURATION_DESCRIPTOR</a> structure.


### -output-buffer-length

Size of the output buffer.


### -in-out-buffer



<text></text>




### -inout-buffer-length



<text></text>




### -status-block

<b>Irp-&gt;IoStatus.Status</b> is set to STATUS_SUCCESS if the request is successful. Otherwise, <b>Status</b> to the appropriate error condition as a <a href="https://msdn.microsoft.com/7792201b-63bb-4db5-803d-2af02893d505">NTSTATUS</a> code. 


## -remarks



<h3><a id="ddk_ioctl_get_usb_descriptor_si"></a><a id="DDK_IOCTL_GET_USB_DESCRIPTOR_SI"></a>DeviceIoControl Parameters</h3>


When the <b>DeviceloControl</b> function is called with the IOCTL_GET_USB_DESCRIPTOR I/O control code, the caller must specify the address of a <a href="..\usbscan\ns-usbscan-_usbscan_get_descriptor.md">USBSCAN_GET_DESCRIPTOR</a> structure as the function's <i>lpInBuffer</i> parameter. Depending on the value specified for the <b>DescriptorType</b> member of the USBSCAN_GET_DESCRIPTOR structure, the function's <i>lpOutbuffer</i> parameter must point to either a <a href="..\usbspec\ns-usbspec-_usb_device_descriptor.md">USB_DEVICE_DESCRIPTOR</a>, <a href="..\usbspec\ns-usbspec-_usb_string_descriptor.md">USB_STRING_DESCRIPTOR</a>, or <a href="..\usbspec\ns-usbspec-_usb_configuration_descriptor.md">USB_CONFIGURATION_DESCRIPTOR</a> structure.

The kernel-mode driver obtains a USB descriptor by calling <a href="https://msdn.microsoft.com/library/windows/hardware/ff538943">UsbBuildGetDescriptorRequest</a>.

For more information, see <a href="https://msdn.microsoft.com/f9216d3c-4930-4c26-8eac-6ee500b038e0">Accessing Kernel-Mode Drivers for Still Image Devices</a>.

For more information about USB descriptors, see the <i>Universal Serial Bus Specification</i>.


