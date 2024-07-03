---
UID: NE:dbgmodel.AddressSpaceRelation
tech.root: debugger
title: AddressSpaceRelation
ms.date: 07/03/2024
targetos: Windows
description: Defines the kind of address space being used.
prerelease: false
req.construct-type: enumeration
req.ddi-compliance: 
req.header: dbgmodel.h
req.include-header: 
req.kmdf-ver: 
req.max-support: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.target-type: 
req.typenames: 
typedef_isUnnamed: false
req.umdf-ver: 
topic_type:
 - apiref
api_type:
 - HeaderDef
api_location:
 - dbgmodel.h
api_name:
 - AddressSpaceRelation
f1_keywords:
 - AddressSpaceRelation
 - dbgmodel/AddressSpaceRelation
dev_langs:
 - c++
helpviewer_keywords:
 - AddressSpaceRelation
---

## -description

Defines the kind of address space being used.

## -enum-fields

### -field Disjoint

The address space is Disjoint.

### -field Equal

The address space is Equal.

### -field Overlapping

The address space is overlapping.

### -field Subset

The address space is a subset.

### -field Superset

The address space is a superset.

## -remarks

USE_CURRENT_HOST_CONTEXT  - Methods which take an IDebugHostContext can be called with this special defined value to indicate to the debug host that the "current" context of the debugger should be used.  This is in lieu of explicitly calling IDebugHost::GetCurrentContext and explicitly passing it to the method needing
an IDebugHostContext.

Using this may be more efficient than the explicit query and pass.

## -see-also

[Debugger Data Model C++ Overview](/windows-hardware/drivers/debugger/data-model-cpp-overview)