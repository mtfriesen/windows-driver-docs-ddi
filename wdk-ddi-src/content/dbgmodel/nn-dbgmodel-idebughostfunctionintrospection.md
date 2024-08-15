---
UID: NN:dbgmodel.IDebugHostFunctionIntrospection
tech.root: debugger
title: IDebugHostFunctionIntrospection
ms.date:  08/15/2024
targetos: Windows
description:  A host optional interface which provides detailed information about a function. (dbgmodel.h)
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
 - IDebugHostFunctionIntrospection
f1_keywords:
 - IDebugHostFunctionIntrospection
 - dbgmodel/IDebugHostFunctionIntrospection
dev_langs:
 - c++
helpviewer_keywords:
 - IDebugHostFunctionIntrospection
---

## -description

The **IDebugHostFunctionIntrospection** interface provides detailed information about a function. This is an optional host interface that the client can implement if they want to get such function details.  
   
## -inheritance  
   
`IDebugHostFunctionIntrospection` inherits from the `IUnknown` interface.  
   
- `IUnknown::QueryInterface`: This method is used to obtain a pointer to an interface implemented by an object. It is called by a client that has a pointer to an interface and needs a pointer to another interface on the same object.  
    - `iid`: A reference to the identifier of the interface being requested.  
    - `iface`: The address of a pointer variable that receives the interface pointer requested in the `iid` parameter. Upon successful return, *iface contains the requested interface pointer.  
   
- `IUnknown::AddRef`: This method increments the reference count for an interface pointer to an object. It should be called for every new copy of a pointer to an interface on an object.  
    
- `IUnknown::Release`: This method decrements the reference count for an interface on a object.   
  
## -remarks  

Any object that is required to provide detailed information about an implemented function should consider implementing the `IDebugHostFunctionIntrospection` interface. Following the rules of COM, the object must also implement `IUnknown`.  

## -see-also

[Debugger Data Model C++ Overview](/windows-hardware/drivers/debugger/data-model-cpp-overview)

