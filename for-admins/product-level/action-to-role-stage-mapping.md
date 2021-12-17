---
description: Map Actions to Roles
---

# Actions to Role Stage Mapping

The purpose of this module is to allocate Actions for the unique combination of Role / Product / Stage. This module will enable you to create and map actions (permissions) to the users which are different for each stage. ****&#x20;

Example - You want to show eligibility to the Sales person only when the case is approved. Hence you can just tick the action for eligibility screen only for the stage which is post approvals.

The actions mapping has to be done for **each** role using this screen. You need to select the Role for which you are going to map the actions. On the bottom, you will see list of stages which are available for the selected institution

## **Step 1:**&#x20;

You need click on the first stage to get the list of Actions and Views\
****

![](https://lh4.googleusercontent.com/QIm5jWFusD1rzOqy7RQLP4Xd1frwVpP45asuaZCjNqjahrORFUaSuf6QtZgtJZ65b3u1yi4qxGpG8vCxg-lqcHgfSvjgZ2OYix8moxtLb0PmUxw8adzdGwLThuPKBWll-c2BsWwy)

## **Step 2:**&#x20;

You can tick the respective Actions / Views for each stage and Role Combination. ****&#x20;

![](https://lh6.googleusercontent.com/xJBU\_Bf6xJQ9lanPdtohzaQHluEusc3a93ebrV98XuQUpXt2Byj-U8lyQ9FnjvrRH-z33d8V8GTpJtRTR\_ZTxq4N8Q28M\_3WzSunTbghk-4CuiR3-Z7jJsOvkSOC\_tmBKg6Hk6Yk)

### **DASHBOARD**

{% hint style="success" %}
Mandatory to [add stage](../institute-level/create-stage-and-status.md) as DASHBOARD. All the actions which are applicable on Dashboard (ex - My queue / Apply ) should be assigned to DASHBOARD
{% endhint %}

{% hint style="warning" %}
If the role has APPLY button action given then giving the case login screens actions to DASHBOARD is mandatory. The reason is that when punching a new case, stage is not available with the UI
{% endhint %}

Below actions are common across stage and has to be given for DASHBOARD stage.&#x20;

* [ ] APPLY
* [ ] ANALYTCS
* [ ] SOBRE
* [ ] MY\_QUEUE
* [ ] ALL\_QUEUE
* [ ] ASSIGN\_QUEUE
* [ ] CASE\_DETAILS (_Mandatory)_
* [ ] LAN\_SEARCH
* [ ] NAV-MENU _(Mandatory)_
* [ ] NAVIGATION _(Mandatory)_

## **Step 3:**&#x20;

Click on Save

## **List of Actions / Views**

Refer to the sheet name with [Actions 2.0](https://docs.google.com/spreadsheets/d/1ldtB2MCJGfb3CsK5edDfcOhLDBYjGUMKt53NJQpNdr8/edit?usp=sharing)****

## **Inter Dependencies in Actions**

* OPTN\_BTN action is mandatory to show all the buttons inside the screen

![](<../../.gitbook/assets/image (59).png>)

* CASE\_LOGIN action is mandatory if the sourcing / demographic screens have to be shown. Otherwise after opening the case, still dashboard will be visible

![](<../../.gitbook/assets/image (60).png>)

\
