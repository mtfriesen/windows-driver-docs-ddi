---
UID: NN:dbgmodel.IDebugHostType4
tech.root: debugger
title: IDebugHostType4
ms.date:  08/15/2024
targetos: Windows
description: The IDebugHostType4 (dbgmodel.h) interface is an IDebugHostSymbol derived interface that provides access to a particular type.
prerelease: false
req.assembly: 
req.construct-type: iface
req.ddi-compliance: 
req.header: dbgmodel.h
req.idl: 
req.include-header: 
req.max-support: 
req.namespace: 
req.redist: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.target-type: 
req.unicode-ansi: 
topic_type:
 - apiref
api_type:
 - COM
api_location:
 - dbgmodel.h
api_name:
 - IDebugHostType4
f1_keywords:
 - IDebugHostType4
 - dbgmodel/IDebugHostType4
dev_langs:
 - c++
helpviewer_keywords:
 - IDebugHostType4
---

## -description

An ([IDebugHostSymbol](nn-dbgmodel-idebughostsymbol.md) derived) interface to a particular type.

A given language/native type is described by the IDebugHostType2 or [IDebugHostType](nn-dbgmodel-idebughosttype.md) interfaces. Note that some of the methods on these interfaces only apply for specific kinds of types.

This version 4 of the interface supports all of the previous methods with identical signatures and includes additional new methods that provide added functionality. The new methods are listed in the header at the end of the section for that interface.

## -remarks

## -see-also

[Debugger Data Model C++ Interfaces Overview](/windows-hardware/drivers/debugger/data-model-cpp-overview)
