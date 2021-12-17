---
description: >-
  This module will help you determine the queue allocation and the column
  headers for the dashboard screen in the GoNoGo
---

# Configure Dashboards

### Description of the Config Screen

![](https://lh4.googleusercontent.com/bOV5a23iddWdUxBKF7hjm6VsN8tBFcj7B8RcpNxO6pgNGwTfa0ZtJWlyFx5fXzb6v6qi-QwmwybmJxOGSiiQ0o0N4YjOZdI-hj35KkKdOQx8HPN\_VQgF38kHJis\_rbgucCcFc0IH)

1. Role and Type of Dashboard
2. Query Builder for dashboard query
3. Selection of column headers

## Section 1

This section will help you select the below things

* Product : Will be read-only
* Role: The role  dropdown will come from the [Sync Role](../../institute-level/sync-products-roles.md#view-roles)
* Type: Will have two values. “MY” and “ALL”. ****&#x20;

## **Section 2 : Query Builder**

![](https://lh6.googleusercontent.com/hQU6A2WgZprZgSo8XEnZxMeXA1Fl50EcGN6s\_18oIST33SBkuSSsmQvOclCDaRJ2KY6QGfgoEKPwo6bVNooLyPQb7GagfT0QwA8nOi9wtBaSyGwBQLgcx-Lf7\_uLVCA4toVWHmRj)

This Section will help you create a query for queue allocation. The list of fields available and their description is below. The fields are of 3 types

* **UI\_request:** This type of fields will take the value dynamically at the time of login. No need to select any value for this equation
* **User Input:** This value will be constant and user can enter it
* **Dropdown:** User needs to select (multi-select) from the dropdown values available

### List of fields&#x20;

Thefields available for query builder are list below

| **Field name** | **Json Path** | **Description** | **Type** |
| -------------- | ------------- | --------------- | -------- |
|                |               |                 |          |
|                |               |                 |          |

### **Operator Types**

| Operator Name      | Desc |
| ------------------ | ---- |
| IN                 |      |
| IS                 |      |
| NOTEQL             |      |
| ELEMENT\_MATCH     |      |
| LESS\_THAN         |      |
| GREATER\_THAN      |      |
| LESS\_THAN\_EQL    |      |
| GREATER\_THAN\_EQL |      |

{% content-ref url="sample-queries.md" %}
[sample-queries.md](sample-queries.md)
{% endcontent-ref %}

## Section 3 : Column Headers

This will help you select the column headers to be show for the respective role.&#x20;

![](https://lh4.googleusercontent.com/oZM8rUefpwWmfWSHVbdjlrDvWya1DkHEdh4oecktll4f-nQ8mkpSv9jix7XNm7ZyxUqdpSizSGj2Gic2h0pgktIWSp03wxMcEduEc2PutEF0TLke7jfuUYssmObU30QylQHsE3jv)

* The Key name will be pre-defined and use has to select from the list available
* The column name can be anything which users wants to show to the users. &#x20;

{% hint style="info" %}
* You can select different columns for each roles
* Ensure you **don't** select more than 6-7 columns otherwise the dashboard will looks dense. &#x20;
{% endhint %}

List of Column Headers available

| Column Name | Desc |
| ----------- | ---- |
|             |      |

## Non Configurable Items

Below items needs to be done by developers&#x20;

* [x] Indexing in queries for each role / product / institute
* [x] Monitoring query performance
