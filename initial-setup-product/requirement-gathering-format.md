---
description: Use the below formats for requirement gathering from customers
---

# Requirement Gathering Format

{% hint style="success" %}
Download the [Format](https://docs.google.com/spreadsheets/d/1\_Vt0\_CLCvmw2OXinuNxu9k84YvD5\_SThQ09kkfGUy1I/edit?usp=sharing)

**Make a copy of the file**
{% endhint %}

### 1. Enter Product Details

### 2. Prepare lists

Prepare lists of below items as a step1 of requirement gathering

* [ ] Roles
* [ ] Stages and Status
* [ ] Select Screens
* [ ] 3rd Party APIs / 1st Party APIs

### 3. Create Workflow and DFD

Add the sequence of stages and its trigger points to change the stage and status.&#x20;

To know more about [triggers](../for-admins/product-level/workflow/#section-2-node-condition)&#x20;

### 4. Access Control for Roles

Map roles with the screens the stages.&#x20;

_Example_ - a role can have 4 screens for one stage and 10 screens for other stage

### **5. Prepare Dashboard Logic**

For each role, enter the dashboard logic to show the cases. For reference use [Dashboard filters](../for-admins/product-level/configure-dashboards/#section-2-query-builder)

### 6. Prepare list of Fields

For all the selected screens, prepare a list of fields for each screen. For master list of fields, you can refer to the [Field Super Set](../for-admins/lentra-level-configs/field-super-set.md) screen in Admin &#x20;

### 7. Validations

Add validations which are present at screen level.&#x20;

**Example** - 2 co-applicant mandatory on Demographic OR Bank Account Verification Mandatory

### 8. Prepare custom fields list

Prepare list of fields which are not part of the super set and still clients requires it on the screen. This new fields can be added using custom objects.&#x20;

