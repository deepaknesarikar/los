---
description: Create Additional Fields for the screens
---

# Custom Objects

Custom Objects help you to create Dynamic fields for the below list of screens

### List of Screens and linkage (supported with custom objects)

| Screen             | Linkage            | Desc                                             |
| ------------------ | ------------------ | ------------------------------------------------ |
| Sourcing           | Application        | On sourcing screen at the bottom                 |
| Demographic        | Applicant          | On demographic for all applications              |
|                    | Individual         | Only for Individual applicants                   |
|                    | NonIndividual      | Only for Non Individual applicants               |
| Legal Verification | Legal Verification | Legal Verification Screen                        |
| Property Valuation | Property Valuation | Property Valuation Screen                        |
| Cam Inputs         | Cam Inputs         | Cam Inputs Screen                                |
| Field Inspection   | Field Inspection   | Field Inspection Screen for all addresses        |
| Sales PD           | Sales PD           | Sales PD                                         |
| Credit PD          | Credit PD          | Credit PD                                        |
| Repayment Details  | NACH               | On Repayment Details if mode of repayment = NACH |
| Collateral         | Collateral         | Collateral                                       |
| Schedule           | Schedule           | Schedule                                         |

### Process to create Custom Objects

Step 1: Click on **"New Custom Object"**

Step2: Select the Screen from the dropdown. Automatically the linkage will get prefilled.&#x20;

{% hint style="info" %}
Refer Linkages functionality in the above table
{% endhint %}

![](<../../.gitbook/assets/image (270).png>)

1. Object Display Name: This is object name which will be displayed on the Screen
2. Object backend name: This will be used for storing in backend. <mark style="color:red;"></mark> _This should not contain any spaces_
3. Select Screen: Select the screen where you want to add custom object
4. Linkage: This determines the position or display logic for the custom object.

Step 3: Click on Multi Row if you want to object to be a list. Check below screen shots to get the effect of multi row checkbox

![Add button enabled if "MultiRow" = true](<../../.gitbook/assets/image (27).png>)

![Add button not available if "MultiRow" = false](<../../.gitbook/assets/image (28).png>)

Step 4: Select the fields to be added in the object. The attributes of the fields are listed below

| **Attribute**        | **Description**                                                                                                               | **Validation**                                                                                                                                                              |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field Name           | Backend Json key name to store in database                                                                                    | <ul><li>Mandatory</li><li>No spaces and numbers allowed</li><li>Unique required within one object</li></ul>                                                                 |
| Display Name         | UI display name                                                                                                               | <ul><li>Mandatory</li></ul>                                                                                                                                                 |
| Data Type            | <p>Type of the field</p><ul><li>Text</li><li>Integer</li><li>Decimal</li><li>Checkbox</li><li>Date</li><li>Dropdown</li></ul> | <ul><li>Mandatory</li></ul>                                                                                                                                                 |
| MaxLength            | Maximum character input validation                                                                                            | <ul><li>Available only if Data type is Text | Integer | Decimal</li><li>Non-mandatory</li></ul>                                                                             |
| Master Linkage       | Enter the master name                                                                                                         | <ul><li>Mandatory if data Type is "Dropdown"</li></ul>                                                                                                                      |
| Mandatory to Fill?   | If true, will make the field mandatory for saving the screen                                                                  | <ul><li>Non-Mandatory</li></ul>                                                                                                                                             |
| Is Dependant Master? | If the Field type is Dropdown, and master is dependant on the parent master then tick this                                    | <ul><li>The master selected in the "Master Linkage" field has to be made <a href="../masters/untitled-1.md#dependent-dropdown-masters">Dependant master</a> first</li></ul> |
| Parent Master        | Select the parent master                                                                                                      | <ul><li>Mandatory if Is dependant Master is marked as true</li></ul>                                                                                                        |

{% hint style="info" %}
Adding atleast one field is mandatory
{% endhint %}

{% hint style="danger" %}
Removing any fields from custom object will stop showing the field for existing cases also where data was entered
{% endhint %}
