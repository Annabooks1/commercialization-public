---
author: joshbax-msft
title: Create a driver only update package
description: Create a driver only update package
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 17b1a17f-d047-4bb4-a511-e94e36c087ee
---

# Create a driver only update package


HCK Studio supports driver only updates using the **Connect** option. This is commonly referred to as the Driver Update Acceptable (DUA) process.

1.  Download a DUA File for the Windows Dev Center Dashboard.

    1.  Sign in to the Dashboard with your Microsoft account.

    2.  On the Dashboard, Click **Manage submissions** and then click the submission ID.

    3.  Click **Download DUA File** and click **Save**.

2.  From HCK Studio, click **Connect**.

3.  Select **Package** option, and then click **Browse** to open the DUA File.

4.  Under **Packaging Options**, select **Driver Update**.

5.  Click **OK**.

6.  On the **Package** tab, add resource files as needed.

7.  Click **Create Package**.

    You now have an updated driver only package. Submit the package to the Dashboard for update. For more information on that process, see [Dashboard help](http://msdn.microsoft.com/library/windows/hardware/br230803) on Windows Dev Center.

 

 






