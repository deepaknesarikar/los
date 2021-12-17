---
description: Masters Less than 1000 records
---

# Dropdown Masters

Dropdown masters are small masters with records less than 1000 records. Dropdown masters are generally used for creating dropdown on the UI. They can be multi dimensional and the schema is flexible. \


### Tagging of Dropdown masters

Dropdown masters can be tagged to below entities

* Products: You can tag the dropdown master to multiple Products so that it becomes available for the selected Product. It is mandatory to tag master to at least one Product&#x20;
* Roles: You can tag the dropdown master to multiple roles so that it becomes available for the selected roles. It is mandatory to tag master to at least one role&#x20;

### Validations

* Dropdown master name has to be unique within one institution
* Upload can be done on .csv and .xls
* Records in the master should be less than 1000

### Master Format for Dropdown values

Below master format has to be followed for all the dropdown masters which are used as dropdown values in a single field.&#x20;

Below is the columns required in the master

| 1st            | value       | Ex - IND (this will be stored in DB)                                       |
| -------------- | ----------- | -------------------------------------------------------------------------- |
| 2nd            | viewValue   | Ex - Individual                                                            |
| 3rd (Optional) | product     | ALL / BL / LAP etc.                                                        |
| 4th (Optional) | filterValue | Ex - Individual (this will be reference value in case of dependant master) |

{% hint style="info" %}
Adding "**ALL**" in the product column will enable you to show the respective value for all the products.&#x20;
{% endhint %}

### Important Dropdown Masters

All important dropdown masters are noted in this [google sheet](https://docs.google.com/spreadsheets/d/1ldtB2MCJGfb3CsK5edDfcOhLDBYjGUMKt53NJQpNdr8/edit#gid=1536947746). Refer tab name = "Master List"

## Dependent Dropdown masters

Dropdown masters can be made dependant on each other (only within a screen) using this feature. Example of this feature

Lets see there are two masters on sourcing screen, Loan Purpose and Scheme. For the selection of loan purpose, the values in scheme dropdown should change. This can be achieved using the dependant dropdown master

Let us take sample values for both the masters

| Loan purpose (parent master) | Scheme (Child master)                                |
| ---------------------------- | ---------------------------------------------------- |
| Marraige                     | <ul><li><p>MAR1 </p><p>MAR2</p><p>MAR3</p></li></ul> |
| Personal                     | <ul><li><p>PER1</p><p>PER2</p></li></ul>             |
| Business                     | <ul><li>BUS1</li></ul>                               |

&#x20;The sample master for above dependancy will be like below

1. The is Dependant Master? Should be ticked. The parent master name should be selected in the schema of Child Master

![](<../../.gitbook/assets/image (272).png>)

2\. Then child master named **Scheme** should be altered / created in the below way. Note: The product column is optional and hence can be added or omitted as per the requirement

| value | viewValue | filterValue |
| ----- | --------- | ----------- |
| MAR1  | MAR1      | Marraige    |
| MAR2  | MAR2      | Marraige    |
| MAR3  | MAR3      | Marraige    |
| BUS1  | BUS1      | Business    |
| PER1  | PER1      | Personal    |
| PER2  | PER2      | Personal    |
