---
UID: NF:portabledevicetypes.IPortableDevicePropVariantCollection.RemoveAt
title: IPortableDevicePropVariantCollection::RemoveAt (portabledevicetypes.h)
description: Learn how the RemoveAt method removes the element stored at the location specified by the given index.
old-location: wpddk\iportabledevicepropvariantcollection_removeat.htm
tech.root: wpd_dk
ms.date: 02/15/2018
keywords: ["IPortableDevicePropVariantCollection::RemoveAt"]
ms.keywords: IPortableDevicePropVariantCollection interface,RemoveAt method, IPortableDevicePropVariantCollection.RemoveAt, IPortableDevicePropVariantCollection::RemoveAt, IPortableDevicePropVariantCollectionRemoveAt, RemoveAt, RemoveAt method, RemoveAt method,IPortableDevicePropVariantCollection interface, portabledevicetypes/IPortableDevicePropVariantCollection::RemoveAt, wpddk.iportabledevicepropvariantcollection_removeat
req.header: portabledevicetypes.h
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
req.lib: PortableDeviceGUIDs.lib
req.dll: 
req.irql: 
targetos: Windows
req.typenames: 
ms.custom: RS5
f1_keywords:
 - IPortableDevicePropVariantCollection::RemoveAt
 - portabledevicetypes/IPortableDevicePropVariantCollection::RemoveAt
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - PortableDeviceGUIDs.lib
 - PortableDeviceGUIDs.dll
api_name:
 - IPortableDevicePropVariantCollection::RemoveAt
---

# IPortableDevicePropVariantCollection::RemoveAt


## -description

Removes the element stored at the location specified by the given index.

## -parameters

### -param dwIndex 

[in]
Specifies the index of the element to be removed.

## -returns

The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The specified index was out of range.

</td>
</tr>
</table>

## -remarks

You must specify a zero-based index.

## -see-also

<a href="/windows-hardware/drivers/ddi/portabledevicetypes/nn-portabledevicetypes-iportabledevicepropvariantcollection">IPortableDevicePropVariantCollection Interface</a>

