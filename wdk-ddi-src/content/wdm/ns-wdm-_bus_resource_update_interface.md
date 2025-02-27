---
UID: NS:wdm._BUS_RESOURCE_UPDATE_INTERFACE
title: _BUS_RESOURCE_UPDATE_INTERFACE (wdm.h)
description: Enables device drivers to make direct calls to parent bus driver routines. This structure defines the GUID_BUS_RESOURCE_UPDATE_INTERFACE interface.
ms.date: 09/30/2018
tech.root: kernel
keywords: ["BUS_RESOURCE_UPDATE_INTERFACE structure"]
ms.keywords: _BUS_RESOURCE_UPDATE_INTERFACE, BUS_RESOURCE_UPDATE_INTERFACE, *PBUS_RESOURCE_UPDATE_INTERFACE,
req.header: wdm.h
req.include-header: 
req.target-type: 
req.target-min-winverclnt: Windows 10, version 1809
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.lib: 
req.dll: 
req.ddi-compliance: 
req.unicode-ansi: 
req.max-support: 
req.typenames: BUS_RESOURCE_UPDATE_INTERFACE, *PBUS_RESOURCE_UPDATE_INTERFACE
targetos: Windows
ms.custom: RS5
f1_keywords:
 - _BUS_RESOURCE_UPDATE_INTERFACE
 - wdm/_BUS_RESOURCE_UPDATE_INTERFACE
 - PBUS_RESOURCE_UPDATE_INTERFACE
 - wdm/PBUS_RESOURCE_UPDATE_INTERFACE
 - BUS_RESOURCE_UPDATE_INTERFACE
 - wdm/BUS_RESOURCE_UPDATE_INTERFACE
topic_type:
 - apiref
api_type:
 - HeaderDef
api_location:
 - wdm.h
api_name:
 - _BUS_RESOURCE_UPDATE_INTERFACE
 - PBUS_RESOURCE_UPDATE_INTERFACE
 - BUS_RESOURCE_UPDATE_INTERFACE
---

# _BUS_RESOURCE_UPDATE_INTERFACE structure


## -description

Enables device drivers to make direct calls to parent bus driver routines. This structure defines the GUID_BUS_RESOURCE_UPDATE_INTERFACE interface.

## -struct-fields

### -field Size

The size, in bytes, of this structure.

### -field Version

The driver-defined interface version. Current version is PCI_FPB_RESOURCE_UPDATE_INTERFACE_VERSION.

### -field Context

A pointer to interface-specific context information.

### -field InterfaceReference

A pointer to an [**InterfaceReference**](nc-wdm-pinterface_reference.md) routine that increments the interface's reference count.

### -field InterfaceDereference

A pointer to an [**InterfaceDereference**](nc-wdm-pinterface_dereference.md) routine that decrements the interface's reference count.

### -field GetUpdatedBusResource

A pointer to the busdriver-implemented callback function that is invoked to retrieve the updated resource information. See [**GET_UPDATED_BUS_RESOURCE**](nc-wdm-get_updated_bus_resource.md)

## -remarks

The BUS_RESOURCE_UPDATE_INTERFACE structure is an extension of the [**INTERFACE**](ns-wdm-_interface.md) structure.

## -see-also

