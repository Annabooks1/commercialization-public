---
title: Step 7 Select and run tests
description: Step 7 Select and run tests
MS-HAID:
- 'p\_sxs\_hlk.step\_4\_\_running\_tests'
- 'p\_sxs\_hlk.proxy\_step\_7\_\_running\_tests'
- 'p\_sxs\_hlk.proxy\_step\_7\_\_select\_and\_run\_tests'
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
Search.SourceType: Video
ms.assetid: 2088B4A0-F83A-4BB0-AD81-AE5E398BF24D
---

# Step 7: Select and run tests


The **Tests** tab displays all of the tests that are associated with the features found on your device. You can filter and sort the listed tests in the following ways:

-   Test Phase Categorization
    -   Bring Up
    -   Development and Integration
    -   Reliability
    -   Tuning and Validation
    -   Manufacturing
    -   Support
        **Note**  In the HLK, test categories replace the level classifications previously used with the HCK. The HLK can be used throughout the product life cycle to test and measure quality at each stage of development.

         
-   Status
-   Test Name
-   Type (manual, non-distributed, special configuration, multiple machine)
    **Note**  You can hover over the test type icons with your mouse for more information about the test types.

     

-   Length
-   Target
-   Machine(s)

**Note**  Manual tests that require user input can interrupt the test process. We recommend that you run manual tests separately from automated tests.

 

**Note**  Some tests require additional input before running. Windows HLK Studio prompts you for more info as needed.

 

The following image shows the Studio **Tests** tab.

![hlk studio tests tab](images/hlk-studio-tests-tab.png)

## <span id="Playlists"></span><span id="playlists"></span><span id="PLAYLISTS"></span>Playlists


Playlists are collections of tests that you can use to define various scenarios in which to test your device. The Windows Hardware Compatibility Program uses an official playlist to determine which devices meet the requirements for compatibility with Windows 10.

<iframe src="https://hubs-video.ssl.catalog.video.msn.com/embed/afc1a262-6147-448f-910c-dbb1bcb18d07/IA?csid=ux-en-us&MsnPlayerLeadsWith=html&PlaybackMode=Inline&MsnPlayerDisplayShareBar=false&MsnPlayerDisplayInfoButton=false&iframe=true&QualityOverride=HD" width="720" height="405" allowFullScreen="true" frameBorder="0" scrolling="no"></iframe>

You can load a playlist by choosing **Load Playlist** from within the **Tests** tab. You can load only one playlist at a time. To choose a different playlist, you must first unload the current playlist by choosing **Unload Playlist** from the **Tests** tab.

The following image shows the **Load Playlist File** dialog.

![load playlist dialog](images/hlk-studio-load-playlist-file-dialog.png)

Once a playlist is loaded, only tests that are applicable to each target are shown in the UI.

Test results against all playlists for a specific target are kept until the target is removed from the project. When a playlist is loaded, any previous test results against that playlist are also loaded.

You can save an existing collection of tests as a playlist by choosing **Save Selected As Playlist**.

## <span id="Running_a_test"></span><span id="running_a_test"></span><span id="RUNNING_A_TEST"></span>Running a test


**Note**  If you want to re-flash the device before running the test, set the ForceReflash\_KitsTemplate parameter in HLK Studio to 1 and specifying the location of the ffu to flash to the device using the ImagePath\_KitsTemplate parameter.

 

**Note**  If using a playlist, be sure to load it before following these steps.

 

1.  Filter the test results by using the **View By** dropdown list.

2.  Check the box next to each test that you want to run.

3.  Run the selected tests by choosing **Run Selected**.

    If any additional input is needed, Windows HLK Studio will prompt you.

    A progress bar appears. A slight delay occurs when you run a test.

**Note**  To learn more about any test, select the test from the list and press **F1** key or right-click and select **Test Description**. To cancel any running test, right-click it and select **Cancel**.

 

As tests complete, the results are displayed in the **Status** column. A green checkmark means that it passed, while a red X means that it failed. The pane on the right displays project summary information, including target(s) selected, operating systems being tested, product types you qualify for, and status of all tests.

To learn more about the different options on this page, see [HLK Studio - Tests Tab](p_hlk.hlk_studio___tests_tab).

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_sxs_hlk\p_sxs_hlk%5D:%20Step%207:%20Select%20and%20run%20tests%20%20RELEASE:%20%287/11/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")




