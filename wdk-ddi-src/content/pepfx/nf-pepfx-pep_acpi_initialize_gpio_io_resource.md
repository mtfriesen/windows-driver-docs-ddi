---
UID: NF:pepfx.PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE
title: PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE function (pepfx.h)
description: The PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE function initializes a platform extension plug-in's (PEP) PEP_ACPI_GPIO_RESOURCE structure.
old-location: kernel\pep_acpi_initialize_gpio_io_resource.htm
tech.root: kernel
ms.date: 04/30/2018
keywords: ["PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE function"]
ms.keywords: PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE, PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE function [Kernel-Mode Driver Architecture], kernel.pep_acpi_initialize_gpio_io_resource, pepfx/PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE
req.header: pepfx.h
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
req.irql: 
targetos: Windows
req.typenames: 
f1_keywords:
 - PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE
 - pepfx/PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - pepfx.h
api_name:
 - PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE
---

# PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE function (pepfx.h)


## -description

The <b>PEP_ACPI_INITIALIZE_GPIO_IO_RESOURCE</b> function initializes a platform extension plug-in's (PEP) <a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_acpi_gpio_resource">PEP_ACPI_GPIO_RESOURCE</a> structure.

## -parameters

### -param Shareable [in]


Indicates if the device can be shared.

### -param CanWake [in]


Indicates if the device can be woken from a low-power state.

### -param PinConfig [in]


A <a href="/windows-hardware/drivers/ddi/pepfx/ne-pepfx-_gpio_pin_config_type">GPIO_PIN_CONFIG_TYPE</a> enumeration value that identifies the GPIO pin configuration type.

### -param DebounceTimeout [in]


Specifies the hardware debounce wait time, in hundredths of milliseconds.

### -param DriveStrength [in]



### -param IoRestriction [in]



### -param ResourceSourceIndex [in]


This parameter should always be zero.

### -param ResourceSourceName [in]


This parameter should always be "ResourceConsumer."

### -param ResourceUsage [in]


Indicates if this device is in use.

### -param VendorData [in]


A pointer to a raw data buffer containing vendor-defined byte data to be decoded by the OS driver.

### -param VendorDataLength [in]


The size of the buffer in the <i>VendorData</i> parameter.

### -param PinTable [in]


A list of pin numbers on the resource.

### -param PinCount [in]


The number of pins described by the <i>PinTable</i> parameter.

### -param Resource [out]


A pointer to the resource. The structure behind the pointer is of type <a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_acpi_gpio_resource">PEP_ACPI_GPIO_RESOURCE</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/pepfx/ne-pepfx-_gpio_pin_config_type">GPIO_PIN_CONFIG_TYPE</a>



<a href="/windows-hardware/drivers/ddi/pepfx/ns-pepfx-_pep_acpi_gpio_resource">PEP_ACPI_GPIO_RESOURCE</a>
