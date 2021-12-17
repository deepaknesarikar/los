---
description: Conduct discussion with the customer
---

# Personal Discussion

This screen can be used for Personal Discussion with the customer. The questions can be asked to the customer and the feedback can be noted down on the screen.&#x20;

The screen has below sections

![](<../../.gitbook/assets/image (92).png>)

| Section           | Desc                                                                                 |
| ----------------- | ------------------------------------------------------------------------------------ |
| LifeStyle Details | This will help you capture details of the customer house and lifestyle               |
| Reference Check   | Multiple Reference can be captured here                                              |
| Business Details  | If customer is self-employed or has business, then those details can be entered here |
| Applicant Details | All Applicant information can be captured here                                       |
| PD details        | The details of who / when has the PD done can be recorded here                       |

## Features

* Mainly a data entry screen for Credit Verification users
* Custom objects can be added on the screen to create / add new fields
* PD cannot be triggered parellely to the users like FI or RCU
* Capture Geolocation Feature : [Read here](../verifications/field-inspection-fi.md#capture-geolocation-feature)

{% hint style="info" %}
There is separate PD screen for [Sales](../sales/sales-personal-discussion.md) users also.&#x20;
{% endhint %}

#### Parellel PD

PD can be triggered to agency users using this fields. Here all the dealers with verification type = PD\_VERIFIER will be shown in the dropdown. User need to select Submitted and send the case to the agency. Agency user can then select Verified to complete the PD verification part

![](<../../.gitbook/assets/image (178).png>)

### Capture Distance between customer address and branch

[Link](../verifications/field-inspection-fi.md#calculate-geolocation-distance-from-branch)

## **Other Details**

| **Item**                                                                                                   | **Link**                                                        |
| ---------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------- |
| List of Fields                                                                                             | link                                                            |
| List of Validations                                                                                        | link                                                            |
| Masters (Dropdown + Standalone)                                                                            | link                                                            |
| Possible Events                                                                                            | <ul><li>save -personal-discussion</li></ul>                     |
| 3PI APIs                                                                                                   | <ul><li>verify-PAN</li><li>SMS OTP</li><li>Email OTP </li></ul> |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | Yes                                                             |
