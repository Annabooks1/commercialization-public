---
title: FirstRunTask
description: FirstRunTask
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: e6fb5c06-bc60-49f7-9179-44fb156c9fe9
ms.prod: W10
ms.mktglfcycl: deploy
ms.sitesec: msdn
---

# FirstRunTask


The `FirstRunTask` setting specifies the background task that is active, or live, by default for a tile when a user signs in to Windows for the first time.

The background task must register the user with Windows Notification Service at first sign-in, and must send notifications to the app’s live tile.

If the region of the current user account is among those in the Start Tile regional layouts, you can use this setting. For more information, see [RegionalOverrides](regionaloverrides-win8-microsoft-windows-shell-setupstarttilesregionaloverrides.md).

## Values


To make a tile live, do one of the following:

-   If your background task is in JavaScript, specify the .js file that implements the IBackgroundTask interface.

-   If your background task is in XAML or C++, specify the class ID for the application.

## Valid Configuration Passes


specialize

auditUser

oobeSystem

## Parent Hierarchy


[Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup-win7-microsoft-windows-shell-setup.md) | [StartTiles](starttiles-win8-microsoft-windows-shell-setupstarttiles.md) | [RegionalOverrides](regionaloverrides-win8-microsoft-windows-shell-setupstarttilesregionaloverrides.md) | [RegionalOverride](regionaloverride-win8-microsoft-windows-shell-setupstarttilesregionaloverridesregionaloverride.md) | [WideTiles](widetiles-win8-microsoft-windows-shell-setupstarttilesregionaloverridesregionaloverridewidetiles.md) | [WideTile3](widetile3-win8-microsoft-windows-shell-setupstarttilesregionaloverridesregionaloverridewidetileswidetile3.md) | **FirstRunTask**

## Applies To


For a list of the Windows® editions and architectures that this component supports, see [Microsoft-Windows-Shell-Setup](microsoft-windows-shell-setup-win7-microsoft-windows-shell-setup.md).

## XML Example


The following XML output shows how to use the `<WideTiles>` component.

``` syntax
     <WideTiles>
          <WideTile1>
               <AppId>12345ChannelFabrikam.channel-ABC_defghij6789!App</AppId>
               <FirstRunTask>backgroundtask.js</FirstRunTask>
          </WideTile1>
          <WideTile2>
               <AppId>34567ChannelFabrikam.channel-DEF_012ghijk345!App</AppId>
               <FirstRunTask>Fabrikam.FirstRunTask</FirstRunTask>
          </WideTile2>
          <WideTile3>
               <AppId>56789ChannelFabrikam.channel-GHI_67890jklmno!App</AppId>
          </WideTile3>
     </WideTiles>
```

## Related topics


[StartTiles](starttiles-win8-microsoft-windows-shell-setupstarttiles.md)

[RegionalOverrides](regionaloverrides-win8-microsoft-windows-shell-setupstarttilesregionaloverrides.md)

[WideTiles](widetiles-win8-microsoft-windows-shell-setupstarttilesregionaloverridesregionaloverridewidetiles.md)

[WideTiles](widetiles-win8-microsoft-windows-shell-setupstarttileswidetiles.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_unattend\p_unattend%5D:%20FirstRunTask%20%20RELEASE:%20%2810/3/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





