---
description: How to solve "Master Not Present" Issue
---

# Solve 'Master Not Present'

This error will be shown in two cases

* Master is really not present in the masters module
* Master loading took more time to load, and  UI screen got loaded first

In any of the cases, you will a dropdown like below

![](<../.gitbook/assets/image (201).png>)

### Steps to troubleshoot

Scenario1 : Master is absent in masters module

1. Check in masters module if the master is present with the same name as shown in the dropdown. Example = in the above image, then 2nd value is the name of the master.&#x20;
2. Copy the name and check in the masters module
3. If master is not present then upload the same master with below columns
   1. `value`
   2. `viewValue`
   3. `product (ALL is supported)`

Scenario2 : Master loaded slow and screen loaded fast

1. Click on refresh Dropdown button
2. The master should load
3. If the master doesnt load, then please refer to scenario-1 (as master should not be present for your institution&#x20;
