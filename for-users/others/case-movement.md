---
description: Submit the case after our work is completed
---

# Case Movement

Case movement will happen on the submit or decision buttons given to the users. The buttons are

* Submit
* Approve
* Decline
* Hold
* Subjective Approval (Inside Option Button)

![](<../../.gitbook/assets/image (124).png>)

The case movement on this button is governed by [Workflow](../../for-admins/product-level/workflow/)



### Wait Screen on SUBMIT button

Whenever there will BRE call plugged in the workflow on the submit button, then UI will show a <mark style="background-color:orange;">60 sec loading</mark> and will wait for sobre to change the stage and status.&#x20;

![Loading screen on submit button](<../../.gitbook/assets/image (278).png>)

#### How to enable this screen

* Add sobreExecutor to the Submit node in [workflow](../../for-admins/product-level/workflow/)
* Add Stage or Status on the [sobre-eligibility mapper](../../for-admins/module-level/eligibility-sobre-mapper.md)

#### Description of Screen

* The screen waits for max 60 sec. If within that time , BRE responds then it will show the stage and status
* If BRE doesnt respond, then after 60 sec the screen will show the same stage and status.&#x20;
* User can go back to the case or can go to dashboard

{% hint style="warning" %}
Whenever Stage or Status is mapped in sobre-eligibility mapper, then stage/ status will get only change in case of sobre response. If sobre doesnt respond then the stage will not get changed **(even using workflow)**

Basically, workflow is not used to change the stage / status if stage status is present in the sobre-eligibility mapper
{% endhint %}

