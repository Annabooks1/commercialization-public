---
title: WEKF\_Scancode.Add
description: WEKF\_Scancode.Add
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: cb5ea693-e871-4338-957a-f78f87a932ba
---

# WEKF\_Scancode.Add


This method adds a new custom scan code combination and enables Keyboard Filter to block the new combination.

## Syntax


``` syntax
[Static] uint32 Add(
    [In] string Modifiers, 
    [In] uint16 Scancode
);
```

## Parameters


<a href="" id="modifers"></a>*Modifers*  
The modifier keys that are part of the key combination to block.

<a href="" id="scancode"></a>*Scancode*  
The hardware scan code of the key to block.

## Return Value


Returns an HRESULT value that indicates [WMI non-error constant](http://go.microsoft.com/fwlink/p/?LinkID=208318) or a [WMI error constant](http://go.microsoft.com/fwlink/p/?LinkID=208317).

## Remarks


**WEKF\_Scancode.Add** creates a new **WEKF\_Scancode** object and sets the **Enabled** property of the new object to **true**.

If a **WEKF\_Scancode** object already exists with same *Modifiers* and *Scancode* properties, then **WEKF\_Scancode.Add** returns an error code and does not create a new object or modify any properties of the existing object. If the existing **WEKF\_Scancode** object has the **Enabled** property set to **false**, Keyboard Filter does not block the scan code.

## Requirements


|                       |           |
|-----------------------|-----------|
| Windows Edition       | Supported |
| Windows 10 Home       | No        |
| Windows 10 Pro        | No        |
| Windows 10 Enterprise | Yes       |
| Windows 10 Education  | Yes       |

 

## Related topics


[WEKF\_Scancode](wekf-scancode.md)

[Keyboard Filter](keyboardfilter.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_enterprise_customizations\p_enterprise_customizations%5D:%20WEKF_Scancode.Add%20%20RELEASE:%20%2810/17/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")





