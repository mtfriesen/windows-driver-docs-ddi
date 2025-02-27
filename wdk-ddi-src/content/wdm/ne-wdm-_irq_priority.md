---
UID: NE:wdm._IRQ_PRIORITY
title: _IRQ_PRIORITY (wdm.h)
description: The _IRQ_PRIORITY enumeration (wdm.h) type indicates the priority the system should give to servicing a device's interrupts.
old-location: kernel\irq_priority.htm
tech.root: kernel
ms.date: 04/30/2018
keywords: ["IRQ_PRIORITY enumeration"]
ms.keywords: "*PIRQ_PRIORITY, IRQ_PRIORITY, IRQ_PRIORITY enumeration [Kernel-Mode Driver Architecture], IrqPriorityHigh, IrqPriorityLow, IrqPriorityNormal, IrqPriorityUndefined, PIRQ_PRIORITY, PIRQ_PRIORITY enumeration pointer [Kernel-Mode Driver Architecture], _IRQ_PRIORITY, kernel.irq_priority, sysenum_a5a51a77-ee9c-4e74-9ee4-b097eb361c18.xml, wdm/IRQ_PRIORITY, wdm/IrqPriorityHigh, wdm/IrqPriorityLow, wdm/IrqPriorityNormal, wdm/IrqPriorityUndefined, wdm/PIRQ_PRIORITY"
req.header: wdm.h
req.include-header: Wdm.h, Ntddk.h, Ntifs.h, Miniport.h
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
targetos: Windows
req.typenames: IRQ_PRIORITY, *PIRQ_PRIORITY
f1_keywords:
 - _IRQ_PRIORITY
 - wdm/_IRQ_PRIORITY
 - PIRQ_PRIORITY
 - wdm/PIRQ_PRIORITY
 - IRQ_PRIORITY
 - wdm/IRQ_PRIORITY
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - wdm.h
api_name:
 - _IRQ_PRIORITY
 - PIRQ_PRIORITY
 - IRQ_PRIORITY
---

# _IRQ_PRIORITY enumeration (wdm.h)


## -description

The <b>IRQ_PRIORITY</b> enumeration type indicates the priority the system should give to servicing a device's interrupts.

## -enum-fields

### -field IrqPriorityUndefined

Specifies that the device does not require any particular priority for its interrupts.

### -field IrqPriorityLow

Specifies that the device's interrupts are of low priority. This setting is appropriate for devices that can tolerate higher-than-normal latency.

### -field IrqPriorityNormal

Specifies that the device's interrupts are of normal priority.

### -field IrqPriorityHigh

Specifies that the device's interrupts are of high priority. This setting is appropriate for devices that require low latency.

## -remarks

The system uses <b>IRQ_PRIORITY</b> to assign IRQLs for devices. For example, it might assign a higher IRQL to a device that has an <b>IRQ_PRIORITY</b> of <b>IrqPriorityHigh</b> than it does to a device that has an <b>IRQ_PRIORITY</b> of <b>IrqPriorityLow</b>.

## -see-also

<a href="/windows-hardware/drivers/ddi/wdm/ns-wdm-_io_resource_descriptor">IO_RESOURCE_DESCRIPTOR</a>

