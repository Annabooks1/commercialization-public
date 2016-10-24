---
title: Key
description: Key
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 66564dca-44bc-4933-9518-d513b05ee3f6
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# Key


`Key` specifies a unique key for the [AssociationElement](microsoft-windows-tabletpc-platform-input-coreassociationdataassociationelement.md).

**Note**  
-   This element does not appear in the **Properties** pane of Windows® System Image Manager (Windows SIM) until you add [AssociationElement](microsoft-windows-tabletpc-platform-input-coreassociationdataassociationelement.md) to the answer file.

-   The value for `Key` is added to the answer file as an attribute of the [AssociationElement](microsoft-windows-tabletpc-platform-input-coreassociationdataassociationelement.md) element. The attribute `wcm:keyValue` is used to identify each unique association. For example, you can specify three different associations by using the `Key` values of **Monitor1**, **Monitor2**, and **Monitor3**.

 

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>Key</em></p></td>
<td><p>Specifies a unique key for the [AssociationElement](microsoft-windows-tabletpc-platform-input-coreassociationdataassociationelement.md). <em>Key</em> is a string.</p></td>
</tr>
</tbody>
</table>

 

This string type does not support empty elements. Do not create an empty value for this setting.

## Valid Configuration Passes


offlineServicing

## Parent Hierarchy


[Microsoft-Windows-TabletPC-Platform-Input-Core](microsoft-windows-tabletpc-platform-input-core-win7-microsoft-windows-tabletpc-platform-input-core.md)| [AssociationData](microsoft-windows-tabletpc-platform-input-coreassociationdata.md)| [AssociationElement](microsoft-windows-tabletpc-platform-input-coreassociationdataassociationelement.md) | **Key**

## Applies To


For a list of the supported Windows editions and architectures that this component supports, see [Microsoft-Windows-TabletPC-Platform-Input-Core](microsoft-windows-tabletpc-platform-input-core-win7-microsoft-windows-tabletpc-platform-input-core.md).

## XML Example


The following XML output shows how to configure `AssociationElement` to associate two Tablet PC monitors to three digitizers on the same system, using the key values: Monitor1, Monitor2, and Monitor3.

``` syntax
<AssociationData>
   <AssociationElement wcm:action="add" wcm:keyValue="Monitor1">&quot;hid#VID_1B96&amp;PID_0008&amp;REV_2100&amp;mi_01&amp;col01&quot;=&quot;PCI\\VEN_8086&amp;DEV_4102&amp;SUBSYS_16B510CF|FUJ5812&quot;</AssociationElement>
   <AssociationElement wcm:action="add" wcm:keyValue="Monitor2">&quot;hid#VID_1B96&amp;PID_0008&amp;REV_2100&amp;mi_01&amp;col02&quot;=&quot;PCI\\VEN_8086&amp;DEV_4102&amp;SUBSYS_16B510CF|FUJ5812&quot;</AssociationElement>
</AssociationData>
   <AssociationElement wcm:action="add" wcm:keyValue="Monitor3">&quot;hid#VID_1B96&amp;PID_0008&amp;REV_2100&amp;mi_01&amp;col03&quot;=&quot;PCI\\VEN_8086&amp;DEV_4102&amp;SUBSYS_16B510CF|FUJ5812&quot;</AssociationElement>
</AssociationData>
```

## Related topics


[AssociationElement](microsoft-windows-tabletpc-platform-input-coreassociationdataassociationelement.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20Key%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





