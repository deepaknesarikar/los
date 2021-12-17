---
description: Map partners and disburse loans together
---

# Co-lending Configs

The loan application can be  sourced and then split in between the partners using the Co-lending configs. Below is the description about how to add configs:&#x20;

### Common Configs

![](<../../.gitbook/assets/image (236).png>)

* **Product Name** : this will auto selected
* **Mark Product for Co-lending**: this flag has to be enabled (Ticked) in order to split the case lender wise. You can turn this off, in case you want to turn co-lending off
* **Max no. of partners**: This will restrict the user to add partner to the maximum specified number
* **Manual Selection of Partner Allowed**: If this is ticked, then the partners can be added deleted manually in gonogo
* **Place of Selection**: By default the partner selection will be available on eligibility screen. If the partner selection has to be given in the [sourcing](../../for-users/sales/sourcing.md#co-lending-section) screen, then you can select Sourcing here. &#x20;

### Addition of Partners

Pre-requisite for partner creation is to Create Partners at institute Level

![](<../../.gitbook/assets/image (237).png>)

&#x20;You can add as many partners as you want for this product . The parameter "Max no. of  partners" will restrict the gonogo user to add partners only till the max limit in gonogo application

**Field Description**

* **Partner**: Partner name coming from from Institute Level
* **Keep Share editable at case level**: This has to be ticked if the partner share and ROI are to be kept editable on the [credit eligibility co-lending pop-up](../../for-users/underwriter/credit-eligibility.md#colending-details)
* **Principal Share** : _Default_ principal share of the partner. This can be edited on gonogo if the "`Keep Share editable at case level`" is ticked
* **Priority** : This will be use in BRE for selecting partner. This field has no significance in case of manual (non BRE) selection of partners
* **Role**: Select all the partner roles. It is recommended to keep seperate roles for each partner. That will allow the the application to identify the partner level decision /remarks
* **ROI** : _Default_ Rate of interest of the partner

For more details about how the configs impact gonogo journey, go through the link below

{% content-ref url="../../for-users/underwriter/credit-eligibility.md" %}
[credit-eligibility.md](../../for-users/underwriter/credit-eligibility.md)
{% endcontent-ref %}

### Additon of Fees for each Partner

![](<../../.gitbook/assets/image (259).png>)

If the fees in application have to be split further for each partner, then the fees name and its split can be added for each partner. You need to click on add button and then add the fee and fee Share.&#x20;

<mark style="background-color:orange;">Notes</mark>:&#x20;

1. The fees dropdown comes from the dropdown master named "feesChargesMaster". If the fees dropdown is blank then
   1. Either the master is not added
   2. The fees for the selected product are not added in the master
2. The Fees Share of all the partners should add together to 100%&#x20;

### Other configurations required

1. All **Role level config** for Partner role: As each partner will have separate role, it would require configs to be added for that role. Below is the list of configs&#x20;
   1. Configure Dashboard ([details](../../for-users/underwriter/credit-eligibility.md#view-colending-pop-up))
   2. Configure Forms
   3. Map Actions View to role
   4. (OPTIONAL) Recommendation / Advance role parameters
2. **Workflow** for changing stage / status after the partner role takes decision (Approve / Decline) on the case.&#x20;
