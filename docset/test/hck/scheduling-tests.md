---
author: joshbax-msft
title: Scheduling Tests
description: Scheduling Tests
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 123971f1-c0ce-4094-b869-02966d2e6fac
---

# Scheduling Tests


Use the **Test.QueueTest()** method to put all your tests in a queue that will run on client computers.

If a test is associated with more than one target (and therefore more than one computer), the test is scheduled so that it runs on the first available computer. Scheduling is limited to computers that are in the correct machine pool at the time of scheduling and are in a ready or running state. If a computer isn't ready at the time of scheduling, the test won't run on that computer.

You can't schedule a test if no computers are found, and you can't add computers that are later available.

 

 






