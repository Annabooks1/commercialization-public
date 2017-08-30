---
title: Camera Driver Controls System Test - Photo Sequence - Max Past Frames
description: Camera Driver Controls System Test - Photo Sequence - Max Past Frames
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 8bd52143-09e7-4340-b623-553310a3a048
---

# <span id="p_hlk_test.3aab27f6-aa75-445b-b6ba-cb0fc6ce0c9c"></span>Camera Driver Controls System Test - Photo Sequence - Max Past Frames


This test validates cameras functionality if the driver supports KSPROPERTY\_CAMERACONTROL\_EXTENDED\_PHOTOMODE; if it does not, you should skip this test.

**Note**  
This is an optional control. If the driver does not support a control, you should not implement a control handler just to return an error. If a control handler is registered, the test expects the control to be fully functional.

 

If the driver implements the control handler, the following checks are run based on the definition of the controls by the camera topics document. (Note: Implementation of extended controls such as photo mode also requires the implementation of other extended controls; see Requirements and the camera topics document for details.)

-   Verifies default values (if appropriate).

-   Validates that a property is advertised on correct pin or filter level.

-   Enumerates possible control values while pins are streaming and not streaming.

-   Determines end-to-end functionality.

Startup latency is checked by the test measures by taking the delta between when the trigger was sent and when the sink received the first frame from the image pin. This is the PhotoSink\_Time that is printed in the log if the test fails.

This test also validates photo frame rate by getting the value that the driver advertises on the get call of KSPROPERTY\_CAMERACONTROL\_EXTENDED\_PHOTOMAXFRAMERATE. The test validates that the frame rate is within 10% of the advertised average frame rate. and that no frames are dropped during the photo sequence operation. Note that the min and max checks validate that a frame is no more than one-half of a frame early or late.

When KSPROPERTY\_CAMERACONTROL\_EXTENDED\_PHOTOMAXFRAMERATE is set by the test, the driver should not exceed the frame rate that is passed in by the application. Note that this is a max frame rate, so the driver can do any frame rate that is lower than the one that is requested. Although when driver is queried for KSPROPERTY\_CAMERACONTROL\_EXTENDED\_PHOTOMAXFRAMERATE, it should report its new value.

This test also validates that KSPROPERTY\_CAMERACONTROL\_EXTENDED\_PHOTOMODE is only advertised on the photo pin. If the driver receives a pin ID other than its photo pin. it should fail with ERROR\_INVALID\_PARAMETER.

## <span id="Test_details"></span><span id="test_details"></span><span id="TEST_DETAILS"></span>Test details


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Specifications</strong></td>
<td><ul>
<li>System.Client.Camera.VideoCaptureAndCameraControls</li>
</ul></td>
</tr>
<tr class="even">
<td><strong>Platforms</strong></td>
<td><ul>
<li>Windows 10 for desktop editions (Home, Pro, Enterprise, and Education) x86</li>
<li>Windows 10 for desktop editions x64</li>
<li>Windows 10 Mobile ARM</li>
<li>Windows 10 for desktop editions ARM64</li>
<li>Windows 10 Mobile ARM64</li>
</ul></td>
</tr>
<tr class="odd">
<td><strong>Supported Releases</strong></td>
<td><ul>
<li>Windows 10</li>
<li>Windows 10, version 1511</li>
<li>Windows 10, version 1607</li>
<li>Windows 10, version 1703</li>
</ul></td>
</tr>
<tr class="even">
<td><strong>Expected run time (in minutes)</strong></td>
<td>15</td>
</tr>
<tr class="odd">
<td><strong>Category</strong></td>
<td>Scenario</td>
</tr>
<tr class="even">
<td><strong>Timeout (in minutes)</strong></td>
<td>25</td>
</tr>
<tr class="odd">
<td><strong>Requires reboot</strong></td>
<td>false</td>
</tr>
<tr class="even">
<td><strong>Requires special configuration</strong></td>
<td>false</td>
</tr>
<tr class="odd">
<td><strong>Type</strong></td>
<td>automatic</td>
</tr>
</tbody>
</table>

 

## <span id="Additional_documentation"></span><span id="additional_documentation"></span><span id="ADDITIONAL_DOCUMENTATION"></span>Additional documentation


Tests in this feature area might have additional documentation, including prerequisites, setup, and troubleshooting information, that can be found in the following topic(s):

-   [System.Client additional documentation](system-client-additional-documentation.md)

## <span id="Running_the_test"></span><span id="running_the_test"></span><span id="RUNNING_THE_TEST"></span>Running the test


Before you run the test, complete the test setup as described in the test requirements: [System Client Testing Prerequisites](system-client-testing-prerequisites.md).

## <span id="Troubleshooting"></span><span id="troubleshooting"></span><span id="TROUBLESHOOTING"></span>Troubleshooting


For generic troubleshooting of HLK test failures, see [Troubleshooting Windows HLK Test Failures](p_hlk.troubleshooting_windows_hlk_test_failures).

For troubleshooting information, see [Troubleshooting System Client Testing](troubleshooting-system-client-testing.md).

## <span id="More_information"></span><span id="more_information"></span><span id="MORE_INFORMATION"></span>More information


### <span id="Parameters"></span><span id="parameters"></span><span id="PARAMETERS"></span>Parameters

| Parameter name                  | Parameter description                                                |
|---------------------------------|----------------------------------------------------------------------|
| **DriverVerifierExcludedFlags** | Driver Verifier flags that may be manually excluded for the test run |

 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_hlk_test\p_hlk_test%5D:%20Camera%20Driver%20Controls%20System%20Test%20-%20Photo%20Sequence%20-%20Max%20Past%20Frames%20%20RELEASE:%20%288/29/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/en-us/default.aspx. "Send comments about this topic to Microsoft")




