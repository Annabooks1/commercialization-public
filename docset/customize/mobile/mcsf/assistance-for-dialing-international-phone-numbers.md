---
title: Assistance for dialing international phone numbers
description: Partners can turn off the international assist feature that helps users with the country codes needed for dialing international phone numbers.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 95f93ca3-0481-46bd-93a0-a63380f87bca
---

# Assistance for dialing international phone numbers


Partners can turn off the international assist feature that helps users with the country codes needed for dialing international phone numbers. This customization is recommended when the device will be sold in a country or region that has multiple IDD (country exit code) values.

If the country or region has multiple IDD values but a default is set, international assist will occasionally be successful. The following lists show the countries and regions that are affected for placing or receiving calls.

-   Multiple IDD values, No Default (rarely successful):

    Belize, Brazil, Cambodia, Columbia, Indonesia, Israel, Korea, Maldives, Mauritius, Mongolia, New Caledonia, Singapore, Solomon Islands, Taiwan, Thailand, Uganda, Uruguay

-   Multiple IDD values, default set (occasionally successful):

    Australia, Costa Rica, Finland, Guatemala

If the international assist feature is turned off, it is also possible to override the MNC and MCC used for SMS. For more information, see [International assisted dialing for SMS](international-assisted-dialing-for-sms.md).

<a href="" id="constraints---firstvariationonly"></a>**Constraints:** FirstVariationOnly  

<a href="" id="instructions-"></a>**Instructions:**  
1.  Create a customization answer file using the contents shown in the following code sample.

    ``` syntax
    <?xml version="1.0" encoding="utf-8" ?>  
    <ImageCustomizations xmlns="http://schemas.microsoft.com/embedded/2004/10/ImageUpdate"  
                         Name="AssistedDialSetting"  
                         Description="Use to set the default state of the international assist feature that helps users with country codes needed for dialing international phone numbers."  
                         Owner=""  
                         OwnerType="OEM"> 
    <Static>
        <Settings Path="Phone/PhoneSettings">  
          <Setting Name="AssistedDialSetting" Value="" />      
        </Settings>  
    </Static>
    </ImageCustomizations>
    ```

2.  Specify an `Owner`.

3.  Set `AssistedDialSetting` to one of the following values:

    <table>
    <colgroup>
    <col width="50%" />
    <col width="50%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th>Value</th>
    <th>Description</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td><p>0 or False</p></td>
    <td><p>Turns off the international assist feature by default</p></td>
    </tr>
    <tr class="even">
    <td><p>1 or True</p></td>
    <td><p>Turns on the international assist feature by default</p></td>
    </tr>
    </tbody>
    </table>

     

    By default, the international assist feature is turned off.

<a href="" id="testing-steps-"></a>**Testing steps:**  
1.  Flash a build containing this customization to a device.

2.  Go to the **Phone** settings screen.

3.  Verify whether the **International assist** option is visible, and if so, whether it is turned on or off.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_phCustomization\p_phCustomization%5D:%20Assistance%20for%20dialing%20international%20phone%20numbers%20%20RELEASE:%20%289/7/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




