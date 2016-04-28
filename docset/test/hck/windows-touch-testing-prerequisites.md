---
author: joshbax-msft
title: Windows Touch Testing Prerequisites
description: Windows Touch Testing Prerequisites
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 94c75373-ccbb-4ca6-bf7d-0095122de72a
---

# Windows Touch Testing Prerequisites


Windows Touch is the multi-touch functionality that is natively supported by the Windows operating system since Windows 7. Devices are devices that work with the Windows Touch device and location platform that is currently available on Windows 8 and Windows 7. There is a set of standards defined in the [Windows Hardware Certification Requirements](http://msdn.microsoft.com/library/windows/hardware/hh748188) document for devices and systems that support Windows Touch. Both automated and manual tests are included in Windows Hardware Certification Kit (Windows HCK) to validate that the touch devices that support Windows Touch meet the quality bar per the hardware requirements.

In addition to the standard self-certification submission for devices through the Windows Hardware Quality Labs (WHQL), partners who are building touch hardware must have the Windows Touch Test Lab (WTTL) run the Windows touch tests on touch devices as the final validation step of hardware certification. This validation step is not required for system submissions.

This section describes the process that you should follow before you start to test a Windows® Touch device by using the Windows® Hardware Certification Kit (Windows HCK) and complete the certification for your touch device.

## <a href="" id="bkmk-labenvironments"></a>Windows Touch Test Lab


Microsoft provides this service free of any additional charge beyond a standard submission fee. Before you submit the touch devices to WTTL for device certification, a passed Windows HCK submission package must be generated and attached through in-house Windows HCK test for touch. Once the submission has been made and the physical touch device has delivered to WTTL, the WTTL will run a complete set of Windows Touch tests in Windows HCK using high-precision assistant jigs and styluses where possible to minimize human error. It attempts each test item up to a maximum of two times.

If the device passes all tests for touch certification, the WTTL passes the submission to allow for certification of the touch device. If any tests fail, the WTTL issues a report that lists the failed tests. The WTTL provides the option for partners to choose whether they want to leave the device with Microsoft for future submissions or return submitted hardware to the sender upon request.

The expected turnaround time for WTTL validation is within eight to ten business days after the WTTL receives the device, assuming no unanticipated device setup issues. WTTL sends email messages to submitting partners when it receives their devices. However, the WTTL may take as long as 10 business days if other devices are waiting for submission validation or the submitted device exhibits unanticipated reliability or setup issues. We recommend that partners reserve reasonable time in their product development cycle for in-house touch testing and the hardware certification process for both devices and systems.

For detail information of Windows Touch Test Lab, see. [Windows Touch Device Certification Processes and Windows Touch Test Lab (WTTL) Service](windows-touch-device-certification-processes-and-windows-touch-test-lab--wttl--service.md).

### Contact devices and fingers

Some of the Windows Touch tests, such as UX (user experience), are expected to pass using freehand operation mainly. WTTL will perform the test by using finger contact. The precision tests will require assistive test tools to avoid human manipulation error. In the assistive test tools, WTTL will use a stylus with a 9.0 millimeter diameter.

### Guidance systems

If you already have mechanical or jig-based systems in your testing laboratory, we encourage you to use those systems to complete the tests where applicable.

For point tests, align the contact device or devices with the required target points, and make contact on the digitizer in a movement that is perpendicular to the touch screen. To reduce issues of parallax, place the eye directly behind the contact device so that the eye, contact device, and target point are all in a line perpendicular to the screen. For the press and hold tasks, keep the contact device steady while you touch the screen.

For the line test, follow the point test guidance when you begin and end the line trace at the indicated start and end points. Trace the line as closely as possible to the target line. Accurate parts of the traced line appear in green, and inaccurate portions appear in red.

### Windows Touch Test Lab validation process

The WTTL follows the following process to validate touch devices for Windows Touch hardware certification qualification:

1.  Set up the device according to the instructions submitted by the partner.

2.  Load WHCK software and necessary drivers for the device to be tested.

3.  Run the applicable touch tests listed for the touch device in the WHCK.

4.  Validate each test, following instructions described in [How to Use the Windows Touch Quality Certification Tests](http://msdn.microsoft.com/library/windows/hardware/hh872969). Microsoft will apply high-precision assistant jigs and 9 mm–diameter round styluses when possible to minimize human error.

5.  Attempt each test item a maximum of two times. If all tests in the same category are successful on any attempt, proceed to the tests in the next category.

### Additional Resources for Windows 8 touch hardware testing

For more information about Input and HID, go to [Input and HID - Architecture and Driver Support](http://msdn.microsoft.com/library/windows/hardware/gg487435).

[Windows Pointer Device Data Delivery Protocol](http://msdn.microsoft.com/library/windows/hardware/br259100) provides information about the Windows Pointer Device for Windows operating systems. It provides guidelines for the use of human interface device (HID) protocol for pointer devices to communicate with the Windows host. This document also talks about the required protocol rules to be HID compliant for Windows 8.

[How to Design and Test Multitouch Hardware Solutions for Windows 8](http://msdn.microsoft.com/library/windows/hardware/hh872968) provides information about how to design and test hardware solutions for Windows Touch. It provides guidelines for independent hardware vendors (IHVs) and original equipment manufacturers (OEMs) to address the quality standards that these hardware solutions must meet so that users have a successful experience with multitouch. It includes associated Windows Hardware Certification touch requirements and how they're tested, as well as guidelines for developers, integrators, and testers of multitouch digitizers and systems to build and test solutions that provide a high-quality user experience and meet the requirements of the Windows Hardware Certification for Touch.

[How to Use the Windows Touch Quality Certification Tests](http://msdn.microsoft.com/library/windows/hardware/hh872969) provides information that will enable an operator to use the Windows Touch Quality Certification Tests to test a piece of Windows® 8 hardware. It discusses the equipment and software that are necessary to run the tests, reviews the content of the suite, and adds general information that should make the tests more useful and easier to apply.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_hck\p_hck%5D:%20Windows%20Touch%20Testing%20Prerequisites%20%20RELEASE:%20%284/27/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




