---
title: ICSPNode GetPropertyIdentifiers
description: ICSPNode GetPropertyIdentifiers
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 8a052cd3-d74c-40c4-845f-f804b920deb4
ms.author: windows-hardware-design-content
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# ICSPNode::GetPropertyIdentifiers

This method returns a list of non-standard properties supported by the node. The returned array must be allocated with `CoTaskMemAlloc`.

## Syntax

``` syntax
HRESULT GetPropertyIdentifiers([out] ULONG* pulCount,
                               [out,size_is(,*pulCount)] GUID** pguidProperties);
```

## Parameters

<a href="" id="pulcount"></a>*pulCount*  
<p style="margin-left: 25px">The number of non-standard properties to return.</p>

<a href="" id="pguidproperties"></a>*pguidProperties*  
<p style="margin-left: 25px">The array of property GUIDs to return. This array must be allocated with `CoTaskMemAlloc`.</p>

## Return Value

A value of S\_OK indicates that the properties were successfully returned. E\_NOTIMPL indicates that this method is not supported by the node.

## Remarks

For externally–transactioned nodes, no additional methods are required for successful rollback.

## Requirements

**Header:** None

## Related topics

[Create a custom configuration service provider](create-a-custom-configuration-service-provider.md)

 





