---
title: SquareOrDesktopTile7
description: SquareOrDesktopTile7
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: d745e91a-b7d9-47e8-803b-88b67c6b7434
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# SquareOrDesktopTile7


`SquareOrDesktopTile7` specifies which application appears as a square tile on the **Start** screen, in position SquareOrDesktopTile7. This position may vary based on the screen size, resolution, and DPI of the target device.

## Child Elements


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>[AppIdOrPath](microsoft-windows-shell-setupstarttilessquaretilessquareordesktoptile7appidorpath.md)</p></td>
<td><p>Specifies the <code>AppID</code> of the Windows Store apps, or the path to the desktop apps, which appear as square tiles on the <strong>Start</strong> screen.</p></td>
</tr>
<tr class="even">
<td><p>[FirstRunTask](microsoft-windows-shell-setupstarttilessquaretilessquareordesktoptile7firstruntask.md)</p></td>
<td><p>Specifies the background task that is active, or live, by default for a tile when a user signs in to Windows for the first time.</p></td>
</tr>
</tbody>
</table>

 

## Valid Configuration Passes


specialize

auditUser

oobeSystem

## Parent Hierarchy


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup-win7-microsoft-windows-shell-setup.md)| [StartTiles](microsoft-windows-shell-setupstarttiles.md) | [SquareTiles](microsoft-windows-shell-setupstarttilessquaretiles.md) | **SquareOrDesktopTile7**

## Applies To


For a list of the Windows® editions and architectures that this component supports, see [Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup-win7-microsoft-windows-shell-setup.md).

## XML Example


The following XML output shows how to use the **SquareTiles** component.

``` syntax
<SquareTiles>
          <SquareOrDesktopTile1>
               <AppIdOrPath>C:\programdata\microsoft\windows\start menu\programs\desktoptile1.lnk</AppIdOrPath>
               <FirstRunTask>backgroundtask.js</FirstRunTask>
          </SquareOrDesktopTile1>
          <SquareOrDesktopTile2>
               <AppIdOrPath>67890ChannelFabrikam.channel-JKL_mnop1234789!App</AppIdOrPath>
               <FirstRunTask>Fabrikam.FirstRunTask</FirstRunTask>
          </SquareOrDesktopTile2>
          <SquareOrDesktopTile3>
               <AppIdOrPath>C:\programdata\microsoft\windows\start menu\programs\desktoptile3.lnk</AppIdOrPath>
          </SquareOrDesktopTile3>
          <SquareTile1>
               <AppId>12345ChannelFabrikam.channel-ABC_defghij6789!App</AppId>
               <FirstRunTask>backgroundtask.js</FirstRunTask>
          </SquareTile1>
          <SquareTile2>
               <AppId>34567ChannelFabrikam.channel-DEF_012ghijk345!App</AppId>
               <FirstRunTask>Fabrikam.FirstRunTask</FirstRunTask>
          </SquareTile2>
          <SquareTile3>
               <AppId>56789ChannelFabrikam.channel-GHI_67890jklmno!App</AppId>
          </SquareTile3>
     </SquareTiles> 
```

## Related topics


[StartTiles](microsoft-windows-shell-setupstarttiles.md)

[RegionalOverrides](microsoft-windows-shell-setupstarttilesregionaloverrides.md)

[SquareTiles](microsoft-windows-shell-setupstarttilesregionaloverridesregionaloverridesquaretiles.md)

[SquareTiles](microsoft-windows-shell-setupstarttilessquaretiles.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20SquareOrDesktopTile7%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





