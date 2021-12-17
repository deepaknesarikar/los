---
description: Screen for case login by entering Application Details
---

# Sourcing

Purpose of sourcing is the capture the basic details of the application and the person who has approached for the loan. These details are used to **generate application ID**.

## **Description**

![Sourcing Screen](<../../.gitbook/assets/image (93).png>)

### **Features**

* This is first screen where journey is going to start.&#x20;
* This screen is **mandatory** for all type of loans
* First Time save on this screen will generate Application ID on the top
* Contact Person / Authorised Signatory will be created as a customer&#x20;
* The sourcing details will be pre-populated from the UAM details. This details come at the time of login. (Ex - Employee ID / Name / Mobile no / Branch name)

{% hint style="warning" %}
SOURCING screen is mandatory for all the applications. Without this the application will not work.&#x20;
{% endhint %}

### Add Contact Person as Co-applicant

![](<../../.gitbook/assets/image (263).png>)

This flag will help you to Navigate the Applicant on sourcing screen  as

* &#x20;By Default, this person will get added as Applicant. Hence if this is not selected (ticked), then the same information will be visible in the Primary Applicant form.&#x20;
* If marked as Co-applicant, then the person will be added as co-applicant
* If it is marked as applicant, then you will get one more option as Mark as Contact Person. This will add the sourcing applicant as contact person

![ ](<../../.gitbook/assets/image (265).png>)

{% hint style="warning" %}
Once ticked and after save, this Tick will get **Disabled.** Also you wont be able to select the co-applicant added using this feature. Therefore the red delete button on co-applicant will be hidden
{% endhint %}

#### Other option in dropdowns

For Fields below, if there is `Other` `OTHER` `Others` as value present in the master then UI will ask for additional input field.

1. Company name
2. Loan purpose &#x20;

## Co-lending Section

If the case is marked as co-lending in the [Co-lending configs](../../for-admins/product-level/co-lending-configs.md#common-configs) AND if the place of selection is Sourcing; then below section will be visible for partner selection for the user&#x20;

![](<../../.gitbook/assets/image (240).png>)

## **Other Details**

| **Item**                                                                                                   | **Link**                                                                                                         |
| ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| List of Fields                                                                                             | link                                                                                                             |
| List of Validations                                                                                        | link                                                                                                             |
| Masters (Dropdown + Standalone)                                                                            | link                                                                                                             |
| Action Name                                                                                                | CL-SOURCING + CASE\_LOGIN                                                                                        |
| Possible Events                                                                                            | <ul><li>register-application</li><li>register-applicant</li><li>dedupe-executor</li><li>sobre-executor</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>verify-PAN</li><li>SMS OTP</li><li>Email OTP </li></ul>                                                  |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | Yes                                                                                                              |

## Andriod App

Andriod app is available for below screens

* All [Sales](./) screens
* All [Verification](../verifications/) Screens

The link is available below

{% hint style="info" %}
APK Link is [here](https://drive.google.com/file/d/13dFBbX3DrBuFZ6sHpGDJJ6OEZVKXrCcu/view?usp=sharing):&#x20;
{% endhint %}
