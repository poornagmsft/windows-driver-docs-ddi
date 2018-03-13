---
UID: NI:ntddvdeo.IOCTL_VIDEO_ENABLE_VDM
title: IOCTL_VIDEO_ENABLE_VDM
author: windows-driver-content
description: This IOCTL is not handled by video miniport drivers. It is handled entirely by the system-supplied video port driver.
old-location: display\ioctl_video_enable_vdm.htm
old-project: display
ms.assetid: 45a5ab64-1b34-4f48-bbe3-285016e9c16e
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: IOCTL_VIDEO_ENABLE_VDM, IOCTL_VIDEO_ENABLE_VDM control code [Display Devices], Video_IOCTLs_d0e75fac-0604-49f5-9293-3455659ab821.xml, display.ioctl_video_enable_vdm, ntddvdeo/IOCTL_VIDEO_ENABLE_VDM
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: ioctl
req.header: ntddvdeo.h
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
-	Ntddvdeo.h
api_name:
-	IOCTL_VIDEO_ENABLE_VDM
product: Windows
targetos: Windows
req.typenames: TAPE_WRITE_MARKS, *PTAPE_WRITE_MARKS
---

# IOCTL_VIDEO_ENABLE_VDM IOCTL


##  Major Code: 


[IRP_MJ_DEVICE_CONTROL](https://docs.microsoft.com/en-us/windows-hardware/drivers/kernel/irp-mj-device-control)

## -description



This IOCTL is not handled by video miniport drivers. It is handled entirely by the system-supplied video port driver.




## -ioctlparameters




### -input-buffer



<text></text>




### -input-buffer-length



<text></text>




### -output-buffer



<text></text>




### -output-buffer-length



<text></text>




### -in-out-buffer



<text></text>




### -inout-buffer-length



<text></text>




### -status-block



Irp->IoStatus.Status is set to STATUS_SUCCESS if the request is successful.

Otherwise, Status to the appropriate error condition as a NTSTATUS code. 

For more information, see [XREF-LINK:NTSTATUS Values].




## -remarks



<div class="alert"><b>Note</b>    This IOCTL is obsolete in Windows Vista.</div>
<div> </div>

