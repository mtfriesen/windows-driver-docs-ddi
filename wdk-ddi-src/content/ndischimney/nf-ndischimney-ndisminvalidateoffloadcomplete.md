---
UID: NF:ndischimney.NdisMInvalidateOffloadComplete
title: NdisMInvalidateOffloadComplete function (ndischimney.h)
description: An offload target calls the NdisMInvalidateOffloadComplete function to complete an invalidate offload operation that was initiated by a previous call to the MiniportInvalidateOffload function of the offload target.
old-location: netvista\ndisminvalidateoffloadcomplete.htm
tech.root: netvista
ms.date: 05/02/2018
keywords: ["NdisMInvalidateOffloadComplete function"]
ms.keywords: NdisMInvalidateOffloadComplete, NdisMInvalidateOffloadComplete function [Network Drivers Starting with Windows Vista], ndischimney/NdisMInvalidateOffloadComplete, netvista.ndisminvalidateoffloadcomplete, tcp_chim_ndis_func_14e16158-2af9-4901-a986-0bfa329d9ac5.xml
req.header: ndischimney.h
req.include-header: Ndischimney.h
req.target-type: Universal
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
req.irql: Any level
targetos: Windows
req.typenames: 
f1_keywords:
 - NdisMInvalidateOffloadComplete
 - ndischimney/NdisMInvalidateOffloadComplete
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - ndischimney.h
api_name:
 - NdisMInvalidateOffloadComplete
---

# NdisMInvalidateOffloadComplete function


## -description

<p class="CCE_Message">[The TCP chimney offload feature is deprecated and should not be used.]

An offload target calls the 
  <b>NdisMInvalidateOffloadComplete</b> function to complete an invalidate offload operation that was
  initiated by a previous call to the 
  <a href="/windows-hardware/drivers/ddi/ndischimney/nc-ndischimney-w_invalidate_offload_handler">
  MiniportInvalidateOffload</a> function of the offload target.

## -parameters

### -param NdisMiniportHandle [in]


The handle that the offload target obtained in a previous call to the 
     <a href="/windows-hardware/drivers/ddi/ndis/nf-ndis-ndismregisterminiportdriver">
     NdisMRegisterMiniportDriver</a> function.

### -param OffloadBlockList [in]


A pointer to an 
     <a href="/windows-hardware/drivers/ddi/ndischimney/ns-ndischimney-_ndis_miniport_offload_block_list">
     NDIS_MINIPORT_OFFLOAD_BLOCK_LIST</a> structure. The offload target obtained this pointer as an input
     parameter to its 
     <a href="/windows-hardware/drivers/ddi/ndischimney/nc-ndischimney-w_invalidate_offload_handler">
     MiniportInvalidateOffload</a> function.

## -remarks

Before calling the 
    <b>NdisMInvalidateOffloadComplete</b> function, the offload target must write either of the following
    NDIS_STATUS values to the 
    <b>Status</b> member of each NDIS_MINIPORT_OFFLOAD_BLOCK_LIST structure in the state tree:

<ul>
<li>
NDIS_STATUS_SUCCESS
     

The offload target successfully invalidated the state objects.

</li>
<li>
NDIS_STATUS_FAILURE
     

The invalidate operation did not succeed. In this case, the offload target has stopped responding (is
     hung).

</li>
</ul>

## -see-also

<a href="/windows-hardware/drivers/ddi/ndischimney/nc-ndischimney-w_invalidate_offload_handler">MiniportInvalidateOffload</a>



<a href="/windows-hardware/drivers/ddi/ndischimney/ns-ndischimney-_ndis_miniport_offload_block_list">
   NDIS_MINIPORT_OFFLOAD_BLOCK_LIST</a>



<a href="/windows-hardware/drivers/ddi/ndis/nf-ndis-ndismregisterminiportdriver">NdisMRegisterMiniportDriver</a>
