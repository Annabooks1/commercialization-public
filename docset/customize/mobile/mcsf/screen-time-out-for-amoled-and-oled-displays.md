---
title: Screen timeout for AMOLED and OLED displays
description: OEMs can remove the 15 minutes, 30 minutes, and Never options from the Screen times out after dropdown in the Lock screen settings screen. This is recommended for phones with AMOLED and OLED screens to prevent screen damage.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 27f5b4e2-6586-4893-a011-23e5f80df9b8
---

# Screen timeout for AMOLED and OLED displays


OEMs can remove the **15 minutes**, **30 minutes**, and **Never** options from the **Screen times out after** dropdown in the **Lock screen** settings screen.

This is recommended for phones with AMOLED and OLED screens to prevent screen damage.

<a href="" id="constraints---firstvariationonly"></a>**Constraints:** FirstVariationOnly  

<a href="" id="instructions-"></a>**Instructions:**  
1.  Create a customization answer file using the contents shown in the following code sample.

    ``` syntax
    <?xml version="1.0" encoding="utf-8" ?>
    <ImageCustomizations xmlns="http://schemas.microsoft.com/embedded/2004/10/ImageUpdate"  
                         Name="ScreenTimeout"  
                         Description="Use to remove the 15 minutes, 30 minutes, and Never options from the screen time-out option in the Lock screen settings screen."  
                         Owner=""  
                         OwnerType="OEM"> 
      
      <Static>  
        <Settings Path="LockScreen">  
          <!-- Set the value to 1 or 0x1 to remove the 15 minutes, 30 minutes, and Never options from the lock screen settings screen -->
          <Setting Name="ScreenTimeOut" Value="" />  
        </Settings>  
      </Static>
    </ImageCustomizations>
    ```

2.  Specify an `Owner`.

3.  To hide or remove the **15 minutes**, **30 minutes**, and **Never** options from the **Screen times out after** dropdown in the **Lock screen** settings screen, set `ScreenTimeOut` to 1 or 0x1.

<a href="" id="testing-"></a>**Testing:**  
1.  Flash the build containing this customization to a phone.

2.  Go to the **lock screen** screen in **Settings**.

3.  Tap the **Screen times out after** setting and verify that the **15 minutes**, **30 minutes**, and **never** options are no longer included in the list.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_phCustomization\p_phCustomization%5D:%20Screen%20timeout%20for%20AMOLED%20and%20OLED%20displays%20%20RELEASE:%20%289/7/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




