---
UID: NC:pep_x.PEPCALLBACKNOTIFYPPM
title: PEPCALLBACKNOTIFYPPM (pep_x.h)
description: Learn how an AcceptProcessorNotification event callback routine handles processor power management (PPM) notifications from the Windows power management framework (PoFx).
old-location: kernel\acceptprocessornotification.htm
tech.root: kernel
ms.date: 04/30/2018
keywords: ["PEPCALLBACKNOTIFYPPM callback function"]
ms.keywords: AcceptProcessorNotification, AcceptProcessorNotification routine [Kernel-Mode Driver Architecture], PEPCALLBACKNOTIFYPPM, kernel.acceptprocessornotification, pepfx/AcceptProcessorNotification
req.header: pep_x.h
req.include-header: Pep_x.h
req.target-type: Windows
req.target-min-winverclnt: Supported starting with Windows 10.
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
req.irql: PASSIVE_LEVEL to HIGH_LEVEL
targetos: Windows
req.typenames: 
f1_keywords:
 - PEPCALLBACKNOTIFYPPM
 - pep_x/PEPCALLBACKNOTIFYPPM
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - UserDefined
api_location:
 - pepfx.h
api_name:
 - PEPCALLBACKNOTIFYPPM
---

# PEPCALLBACKNOTIFYPPM callback function (pep_x.h)


## -description

An <i>AcceptProcessorNotification</i> event callback routine handles processor power management (PPM) notifications from the Windows <a href="/windows-hardware/drivers/ddi/_kernel/#device-power-management">power management framework</a> (PoFx).

## -parameters

### -param Handle 

[in]
The device handle for the PEP for the target processor. If <b>NULL</b>,  the notification does not target a specific processor.

### -param Notification 

[in]
The PPM notification ID. This parameter specifies the type of PPM notification that PoFx is sending. For a list of PPM notification IDs, see <a href="/windows-hardware/drivers/ddi/index">Processor power management (PPM) notifications</a>.

### -param Data 

[in, out, optional]
A pointer to a PoFx-allocated structure that contains the input and/or output data for this notification. The type of this structure depends on the notification ID specified by <i>Notification</i>. For a list of the structure types that are defined for the various PPM notification IDs, see <a href="/windows-hardware/drivers/ddi/index">Processor power management (PPM) notifications</a>.

## -returns

The <i>AcceptProcessorNotification</i> routine must return TRUE if it handles the notification, or FALSE if it does not.

## -remarks

This routine is implemented by the platform extension plug-in (PEP) for a processor. The <b>AcceptProcessorNotification</b> member of the <a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_information">PEP_INFORMATION</a> structure is a pointer to an <i>AcceptProcessorNotification</i> routine. The PEP calls the <a href="/windows-hardware/drivers/ddi/pepfx/nf-pepfx-pofxregisterplugin">PoFxRegisterPlugin</a> or <a href="/windows-hardware/drivers/ddi/pepfx/nf-pepfx-pofxregisterpluginex">PoFxRegisterPluginEx</a> routine to register the PEP's <i>AcceptProcessorNotification</i> routine with PoFx.

The IRQL at which the PEP's <i>AcceptProcessorNotification</i> routine is called varies according to the type of notification that is being sent. The context in which this interface is called ranges from PASSIVE_LEVEL to HIGH_LEVEL with interrupts disabled. For more information about the IRQL at which each notification type is sent, see the individual reference pages under <a href="/windows-hardware/drivers/ddi/index">Processor power management (PPM) notifications</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_information">PEP_INFORMATION</a>



<a href="/windows-hardware/drivers/ddi/pepfx/nf-pepfx-pofxregisterplugin">PoFxRegisterPlugin</a>



<a href="/windows-hardware/drivers/ddi/pepfx/nf-pepfx-pofxregisterpluginex">PoFxRegisterPluginEx</a>

