---
title: CountryOrRegionID
description: CountryOrRegionID
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 8db03f6a-0c71-4ae4-9b27-870207890216
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# CountryOrRegionID


`CountryOrRegionID` specifies the region code for a region that, when selected, shows a set of region-specific apps that appear on the Start and Lock screens.

Each regional override can be used for multiple regions. For example, you could add a set of apps that are designed for South American business travel that only appear for your users in South America.

Your user’s region can be selected by the user during OOBE, or can be specified with Microsoft-Windows-International-Core\\[UserLocale](microsoft-windows-international-coreuserlocale.md).

If the selected region matches a region in Windows-Shell-Setup\\StartMenu\\RegionalOverrides\\RegionalOverride\\Regions\\[Region](microsoft-windows-shell-setup-starttiles-regionaloverridesregionaloverrideregionsregion.md), then Windows displays the set of apps from that regional override. The set of apps is specified by Microsoft-Windows-Shell-Setup\\StartTiles\\RegionalOverrides\\[RegionalOverride](microsoft-windows-shell-setup-starttiles-regionaloverridesregionaloverride.md): WideTiles, SquareTiles, and LockScreen.

If the selected region doesn’t match any of these regions, then Windows displays the set of apps from Microsoft-Windows-Shell-Setup\\[StartTiles](microsoft-windows-shell-setup-starttiles.md): WideTiles, SquareTiles, and LockScreen.

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><em>CountryOrRegionID</em></p></td>
<td><p>Specifies the two-letter country or region ID of the end user (for example, US, FR, ES).</p>
<p>For the list of valid values for <em>CountryOrRegionID</em>, see [http://go.microsoft.com/fwlink/?LinkId=255198](http://go.microsoft.com/fwlink/?LinkId=255198).</p>
<p>This value is not case-sensitive.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


specialize

auditUser

oobeSystem

## Parent Hierarchy


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup.md) | [StartTiles](microsoft-windows-shell-setup-starttiles.md) | [RegionalOverrides](microsoft-windows-shell-setup-starttiles-regionaloverrides.md) | [RegionalOverride](microsoft-windows-shell-setup-starttiles-regionaloverridesregionaloverride.md)| [Regions](microsoft-windows-shell-setup-starttiles-regionaloverridesregionaloverrideregions.md) | [Region](microsoft-windows-shell-setup-starttiles-regionaloverridesregionaloverrideregionsregion.md) | **CountryOrRegionID**

## XML Example


The following XML output shows how to configure a set of Apps that apply to only in France and Italy.

``` syntax
<RegionalOverrides>
  <RegionalOverride>
    <Order>1</Order>
    <Regions>
      <Region>
        <CountryOrRegionID>IT</CountryOrRegionID>
        <Key>1</Key>
      </Region>
      <Region>
        <CountryOrRegionID>FR</CountryOrRegionID>
        <Key>2</Key>
      </Region>
     </Regions>
    <!-- Square tiles, Wide Tiles, and LockScreen apps are specified here -->
  </RegionalOverride>
</RegionalOverrides>
```

## Related topics


[How to Customize the Start Screen](http://go.microsoft.com/fwlink/?LinkId=254187)

[Region](microsoft-windows-shell-setup-starttiles-regionaloverridesregionaloverrideregionsregion.md)

[StartTiles](microsoft-windows-shell-setup-starttiles.md)

[UserLocale](microsoft-windows-international-coreuserlocale.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20CountryOrRegionID%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





