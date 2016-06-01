---
author: joshbax-msft
title: Distributing Tests
description: Distributing Tests
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 3f1e6239-91fe-497b-8a17-bf6289a30ce6
---

# Distributing Tests


You can run a test on all the targets in a **TargetFamily**, or you can run a test on a subset of **TargetFamily** targets.

Note that there is no hierarchical relationship from **TargetFamily** to **Target** to tests. If you try to create such a hierarchy, all your distributable tests and their results will be duplicated. Also, the **Target.GetTestResults()** method might return results from the wrong target.

Here's an example test distribution:

![target family](images/hck-win8-om-targetfamily.png)

System tests are also distributable. The hardware Id for systems is always **\[SYSTEM\]**.

 

 






