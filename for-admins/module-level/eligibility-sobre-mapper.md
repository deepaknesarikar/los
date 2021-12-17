---
description: Map the Sobre response to eligibilty
---

# Eligibility Sobre Mapper

The Mapper will help the users to map the sobre response in the eligibility (both [credit](../../for-users/underwriter/credit-eligibility.md) and [sales](../../for-users/sales/sales-eligibility.md))

### Step to create Sobre Policy

* Enter the policy Name

{% hint style="info" %}
The policy name has to be added at two places

* In sobre
* In workflow in the [interface](../product-level/workflow/#section-4-interface-configuration) Configurations
{% endhint %}

* Select the product for which policy will be executed
* Select Request Parameters: select the sections which are supposed to go to Sobre in this policy. <mark style="background-color:orange;">Details</mark> are present [here](https://docs.google.com/document/d/1A746NN8YTyx2yIlcrgJJDU9P5kABtOQ0H5yer-o\_cZA/edit?usp=sharing)

![](<../../.gitbook/assets/image (43).png>)

### Mapping Response to Eligibility

On the below screen,

* Left hand side is sobre response (SOURCE)
* Right hand side is Eligibility fields (DESTINATION)

![](<../../.gitbook/assets/image (42).png>)

#### How to add Source (Sobre) fields

* **Type**: Select the type of the sobre field

| Type               | From Key | To key       |
| ------------------ | -------- | ------------ |
| Eligibility-Mapper | Required | Required     |
| Stage              | Required | Not Required |
| Status             | Required | Not Required |
| Remarks            | Required | Not required |
| Mandatory-Mapper   | Required | Required     |

* **From Key:** Enter the field name in this json object.&#x20;
  * For that, you click on check response ![](<../../.gitbook/assets/image (45).png>) to see the latest sobre response json.&#x20;
  * Enter the refId for which sobre has been triggerred
  * Copy the field and the path of the field from the popup and then paste in the source "From Key". Ex - If the field is inside summary, enter summary.APPLICANT-DECISION&#x20;
  * For <mark style="background-color:orange;">more details</mark> about mapping fields of sobre, please refer to this [document](https://docs.google.com/document/d/1A746NN8YTyx2yIlcrgJJDU9P5kABtOQ0H5yer-o\_cZA/edit?usp=sharing)

![Process of Copying sobre field to eligibility](<../../.gitbook/assets/screen-capture (3).gif>)

#### How to add Destination (eligibility) fields

* **To Key:** Select the To Key from the dropdown. For that you need to understand the [data model](../../for-users/sales/sales-eligibility.md#data-model) of eligibility
* **Index**: \[Depricated]
* **Additional Key**: This field is to be entered if any field is added in the additional properties of eligibility. The input value will be shown on the UI.&#x20;

### Important points

{% hint style="info" %}
All the Excess fields on the screen after mapping is done, needs to be removed using the configure forms
{% endhint %}

{% hint style="info" %}
Understanding the data model and screen structure is very important
{% endhint %}

### How to Extract Sobre Request for any ReferenceID

1. Go to Module Config. Click on "DB Query Module".&#x20;
2. Select the collection name as "`sobreResponseLog`". Enter the Reference ID
3. Wait till you get the response
4. Copy the value of `oSobreRequest` from the json
5. **Note**: You might get multiple oSobreRequest. In that case check the timestamp (`dCallDate`)&#x20;

![](<../../.gitbook/assets/image (273).png>)
