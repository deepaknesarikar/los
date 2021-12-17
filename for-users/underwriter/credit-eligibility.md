---
description: Final eligibility of the application
---

# Credit Eligibility

This screen is used as a final eligibility screen and the values in this screen will be used in all the further journey of the case.&#x20;

{% hint style="info" %}
The values like Approved Amount / ROI / Tenure / EMI will be used in all the other screens from this screen itself
{% endhint %}

## Description

The screen contains fields which are in below hierarchy

![](<../../.gitbook/assets/image (102).png>)

structure.&#x20;

![Application level](<../../.gitbook/assets/image (103).png>)

![Applicant / Program level](<../../.gitbook/assets/image (104).png>)



### Data Model

[Same as Sales Eligibility](../sales/sales-eligibility.md)

### Features

* To populate any sobre Fields in the screen, use the [Sobre-Eligibility Mapper](../../for-admins/module-level/eligibility-sobre-mapper.md)
* The extra fields can be hidden using the form config.&#x20;
* For giving multiple eligibility use the Program level fields.&#x20;
* Any field additional field is also supported at all levels
* Clicking on additional properties will open a pop-up to show the additional fields
* Document upload Option is available below the Applicant section ![](<../../.gitbook/assets/image (255).png>) ![](<../../.gitbook/assets/image (105).png>)

## View Colending Pop-up

This pop-up will be seen only if the product is marked for co-lending in [Admin module ](../../for-admins/product-level/co-lending-configs.md)

The pop-up will contain below action items (refer to the numbers in the screenshot)&#x20;

![](<../../.gitbook/assets/image (262).png>)

1. Select Partner: This will give you option to add / remove the partners for this case. If the partner selection is going to happen from BRE, then this button can be made read-only from the co-lending configs
2. Validate Split: This button will calculate the split for all the partners including the self. After every addition / deletion / declined by any partner, Pressing Validate Split is mandatory.  That will ensure that the sum of principal split is always 100%
3. Save: This will save the data as well as the selected partner and his role. This is important for pushing the case to the partner role.&#x20;
4. View Decision: all the decisions taken by the partner roles and their remarks will be visible in this popup (refer below)

![](<../../.gitbook/assets/image (239).png>)

5\. Partner Role Selection: All the added partners will be visible here in dropdown. User can select one partner the respective role of that partner so that the case can be sent. Refer [Co-lending Configs](../../for-admins/product-level/co-lending-configs.md) for mapping partner and its roles

6\. Update Role: Once the partner and partner role are selected click on the Update loan button. The case will be sent to the respective role

{% hint style="warning" %}
In dashboard query: currentCoLendingPartnerRole should be added for the selected role. Then only the case will be visible in the dashboard
{% endhint %}

7\. Fees Split: If the fees are added in the [Fees Charges screen](../operations/fees-and-charges.md) and if the [configs](../../for-admins/product-level/co-lending-configs.md#additon-of-fees-for-each-partner) for fees split are added then the divided fees will also be shown in the pop-up below

![](<../../.gitbook/assets/image (268).png>)

## **Other Details**

| **Item**                                                                                                   | **Link**                                                    |
| ---------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| List of Fields                                                                                             | link                                                        |
| List of Validations                                                                                        | link                                                        |
| Masters (Dropdown + Standalone)                                                                            | link                                                        |
| Possible Events                                                                                            | <ul><li>save-eligibility</li><li>sobre-executorv2</li></ul> |
| 3PI APIs                                                                                                   | NA                                                          |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                                          |
