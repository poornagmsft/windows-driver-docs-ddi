---
UID: NS:ntddndis._NDIS_PCI_DEVICE_CUSTOM_PROPERTIES
title: "_NDIS_PCI_DEVICE_CUSTOM_PROPERTIES"
author: windows-driver-content
description: The NDIS_PCI_DEVICE_CUSTOM_PROPERTIES structure defines the type and speed of the PCI bus that a NIC is running on.
old-location: netvista\ndis_pci_device_custom_properties.htm
old-project: netvista
ms.assetid: fd61184f-0502-492d-9014-6afbfd70c189
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: "*PNDIS_PCI_DEVICE_CUSTOM_PROPERTIES, NDIS_PCI_DEVICE_CUSTOM_PROPERTIES, NDIS_PCI_DEVICE_CUSTOM_PROPERTIES structure [Network Drivers Starting with Windows Vista], PNDIS_PCI_DEVICE_CUSTOM_PROPERTIES, PNDIS_PCI_DEVICE_CUSTOM_PROPERTIES structure pointer [Network Drivers Starting with Windows Vista], _NDIS_PCI_DEVICE_CUSTOM_PROPERTIES, ndis_pci_properties_ref_46b46f9e-32d9-47fb-ad16-bb8b56a5d5bd.xml, netvista.ndis_pci_device_custom_properties, ntddndis/NDIS_PCI_DEVICE_CUSTOM_PROPERTIES, ntddndis/PNDIS_PCI_DEVICE_CUSTOM_PROPERTIES"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ntddndis.h
req.include-header: Ndis.h
req.target-type: Windows
req.target-min-winverclnt: Supported in NDIS 6.0 and later.
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
-	ntddndis.h
api_name:
-	NDIS_PCI_DEVICE_CUSTOM_PROPERTIES
product: Windows
targetos: Windows
req.typenames: NDIS_PCI_DEVICE_CUSTOM_PROPERTIES, *PNDIS_PCI_DEVICE_CUSTOM_PROPERTIES
---

# _NDIS_PCI_DEVICE_CUSTOM_PROPERTIES structure


## -description


The NDIS_PCI_DEVICE_CUSTOM_PROPERTIES structure defines the type and speed of the PCI bus that a NIC
  is running on.


## -syntax


````
typedef struct _NDIS_PCI_DEVICE_CUSTOM_PROPERTIES {
  NDIS_OBJECT_HEADER Header;
  UINT32             DeviceType;
  UINT32             CurrentSpeedAndMode;
  UINT32             CurrentPayloadSize;
  UINT32             MaxPayloadSize;
  UINT32             MaxReadRequestSize;
  UINT32             CurrentLinkSpeed;
  UINT32             CurrentLinkWidth;
  UINT32             MaxLinkSpeed;
  UINT32             MaxLinkWidth;
#if ((NTDDI_VERSION >= NTDDI_WIN7) || NDIS_SUPPORT_NDIS620)
  UINT32             PciExpressVersion;
  UINT32             InterruptType;
  UINT32             MaxInterruptMessages;
#endif 
} NDIS_PCI_DEVICE_CUSTOM_PROPERTIES, *PNDIS_PCI_DEVICE_CUSTOM_PROPERTIES;
````


## -struct-fields




### -field Header

The 
     <a href="..\ntddndis\ns-ntddndis-_ndis_object_header.md">NDIS_OBJECT_HEADER</a> structure for the
     NDIS_PCI_DEVICE_CUSTOM_PROPERTIES structure. NDIS sets the 
     <b>Type</b> member of the structure that 
     <b>Header</b> specifies to NDIS_OBJECT_TYPE_DEFAULT, the 
     <b>Revision</b> member to NDIS_OBJECT_TYPE_PCI_DEVICE_CUSTOM_PROPERTIES_REVISION_1, and the 
     <b>Size</b> member to 
     sizeof(NDIS_PCI_DEVICE_CUSTOM_PROPERTIES).


### -field DeviceType

The PCI device type. For example, conventional, PCI-X, PCI-E, and so on. See the definitions for
     DevProp_PciDevice_DeviceType_xxx in pciprop.h.


### -field CurrentSpeedAndMode

The speed and mode of conventional PCI or PCI-X devices. For conventional PCI devices, see the
     definitions for DevProp_PciDevice_CurrentSpeedAndMode_Pci_Conventional_xxx. For PCI-X devices, see the
     definitions for DevProp_PciDevice_CurrentSpeedAndMode_Pci_X_xxx. This property is valid only for
     conventional PCI and PCI-X devices.


### -field CurrentPayloadSize

The current payload size in the transaction layer for a PCI Express device. See definitions for
     DevProp_PciExpressDevice_PayloadOrRequestSize_xxx. This property is valid only for PCI Express
     devices.


### -field MaxPayloadSize

The maximum payload size in the transaction layer that is supported by a PCI Express device. See
     definitions for DevProp_PciExpressDevice_PayloadOrRequestSize_xxx. This property is valid only for PCI
     Express devices.


### -field MaxReadRequestSize

The maximum read request size for a PCI Express device. See definitions for
     DevProp_PciExpressDevice_PayloadOrRequestSize_xxx. This property is valid only for PCI Express
     devices..


### -field CurrentLinkSpeed

The current link speed for the device. This property is applicable to a PCI Express device. See
     the definitions for DevProp_PciExpressDevice_LinkSpeed_xxx. This property is valid only for PCI Express
     devices.


### -field CurrentLinkWidth

The current link width of the device. This property is applicable to a PCI express device. See the
     definitions for DevProp_PciExpressDevice_LinkWidth_xxx. This property is valid only for PCI Express
     devices.


### -field MaxLinkSpeed

The maximum link speed of an express link for a PCI Express device. See the definitions for
     DevProp_PciExpressDevice_LinkSpeed_xxx. This property is valid only for PCI Express devices..


### -field MaxLinkWidth

The maximum link width that is implemented by an express link for a PCI Express device. See the
     definitions for DevProp_PciExpressDevice_LinkWidth_xxx. This property is valid only for PCI Express
     devices.


### -field PciExpressVersion

The specification version to which an PCI Express device was built. See the definitions for
     DevProp_PciExpressDevice_Spec_Version_xxx. This property is valid only for PCI Express devices.


### -field InterruptType

The hardware support for interrupts on the PCI Express device. See the definitions for
     DevProp_PciDevice_InterruptType_xxx. This property is valid only for PCI Express devices.


### -field MaxInterruptMessages

The number of message interrupts that a PCI Express device supports in hardware. See the
     definition for DevProp_PciDevice_InterruptMessageMaximum. This property is valid only for PCI Express
     devices that support message interrupts.


## -remarks



Some high performance miniport adapters can adjust the hardware configuration and resource allocation
    based on the type and speed of the PCI bus that the NIC is running on. To provide miniport drivers with
    this information during initialization, NDIS queries the custom PCI properties of PCI adapters and
    provides the results in 
    <b>PciDeviceCustomProperties</b> member of the 
    <a href="..\ndis\ns-ndis-_ndis_miniport_init_parameters.md">
    NDIS_MINIPORT_INIT_PARAMETERS</a> structure. The type and speed of the PCI bus is also available
    through the 
    <a href="https://docs.microsoft.com/en-us/windows-hardware/drivers/network/oid-gen-pci-device-custom-properties">
    OID_GEN_PCI_DEVICE_CUSTOM_PROPERTIES</a> OID request and the 
    <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff566745">
    GUID_NDIS_GEN_PCI_DEVICE_CUSTOM_PROPERTIES</a> WMI GUID.




## -see-also

<a href="https://docs.microsoft.com/en-us/windows-hardware/drivers/network/oid-gen-pci-device-custom-properties">
   OID_GEN_PCI_DEVICE_CUSTOM_PROPERTIES</a>



<a href="..\ndis\ns-ndis-_ndis_miniport_init_parameters.md">NDIS_MINIPORT_INIT_PARAMETERS</a>



<a href="..\ntddndis\ns-ntddndis-_ndis_object_header.md">NDIS_OBJECT_HEADER</a>



<a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff566745">
   GUID_NDIS_GEN_PCI_DEVICE_CUSTOM_PROPERTIES</a>



 

 

<a href="mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback [netvista\netvista]:%20NDIS_PCI_DEVICE_CUSTOM_PROPERTIES structure%20 RELEASE:%20(2/26/2018)&amp;body=%0A%0APRIVACY STATEMENT%0A%0AWe use your feedback to improve the documentation. We don't use your email address for any other purpose, and we'll remove your email address from our system after the issue that you're reporting is fixed. While we're working to fix this issue, we might send you an email message to ask for more info. Later, we might also send you an email message to let you know that we've addressed your feedback.%0A%0AFor more info about Microsoft's privacy policy, see http://privacy.microsoft.com/en-us/default.aspx." title="Send comments about this topic to Microsoft">Send comments about this topic to Microsoft</a>
