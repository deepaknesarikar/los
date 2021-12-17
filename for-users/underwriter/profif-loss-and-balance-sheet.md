---
description: Calculate Financials for the applicants
---

# Profit Loss and Balance Sheet

This screen will support fully customizable Profit Loss (PL) and Balance Sheet (BS) formats.

{% hint style="info" %}
The format currently can be customised at product level. Ex - One format for Business loan and different format for Personal loan.&#x20;
{% endhint %}

## Description

The screen has 4 sections to it

* PL
* BS
* Ratio Analysis: This is **derived** from the the input values of the PL and BS by using [calculation config](../../for-admins/module-level/pl-bs-calculations.md)
* Cashflow: This is **derived** from the the input values of the PL and BS by using [calculation config](../../for-admins/module-level/pl-bs-calculations.md)

![PL BS sections](<../../.gitbook/assets/image (113).png>)

### Features

* The fields, their sequence and names can be chosen by the client. The process of [configuring format](profif-loss-and-balance-sheet.md#how-to-configure-pl-bs-formats) is given below
* The formulas can be entered for all the fields in the PL and BS respectively.&#x20;
* The formulas can also be used to create ratios and cashflow fields. For this [calculation config](../../for-admins/module-level/pl-bs-calculations.md) can be used.&#x20;
* There will be a calculate button at the bottom.  ![](<../../.gitbook/assets/image (114).png>) This button has to be used to calculate the fields first and then save them.&#x20;
* Multiple years can be added for the PL BS.&#x20;

### How to configure PL BS formats

1. Go through the field [list](https://docs.google.com/spreadsheets/d/1IglZEQdGhD9mNCDpj0mOc1UQOEUzSpwtCivEIsZFgd4/edit?usp=sharing) and select the applicable fields for your format
2. Use the below attributes in the form config to configure the format

| Attribute      | Desc                                           | Use                                                                                                                                                                                                                                                                    |
| -------------- | ---------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| hidden         | If True will hide the field.                   | Make it true for all the fields which you **don't** want in the format                                                                                                                                                                                                 |
| disabled       | If true, will make the field read-only         | Make it true for all the fields which have formulas entered in them. So that users can only input the fields which are required.                                                                                                                                       |
| placeholder    | Change the name of the field using placeholder | <p>Change the name as per the requirement. </p><p>Ex1- if Profit is the field name, you can change it to Net Income. </p><p>Ex2- use this field to denote hierarchy in the fields. You can "-' or "...." in front of the fields to indent them to denote hierarchy</p> |
| master linkage | Change the sequence of the fields              | This has to be numeric integer input starting from 1                                                                                                                                                                                                                   |
| category       | Will help to make a field bold                 | Change to Section if you want field to be bold. If you want no emphasis then keep it as field.                                                                                                                                                                         |

#### Example

![](<../../.gitbook/assets/image (115).png>)

| Field name                       | How to configure                                                                                                                       | Formula |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | ------- |
| Gross Sales                      | Master Linkage = 1 \| Category = Section \| Placeholder = Gross Sales \| hidden = false \| disabled = true                             | Yes     |
| Export Sales                     | Master Linkage = 2 \| Category = Field \| Placeholder = - - - -Export Sales \| hidden = false \| disabled = false                      | -       |
| Gross Domestic Sales             | Master Linkage = 3 \| Category = Field \| Placeholder = - - - -Gross Domestic Sales \| hidden = false \| disabled = false              | -       |
| Excise Duty                      | Master Linkage = 4 \| Category = Field \| Placeholder = Excise Duty \| hidden = false \| disabled = false                              | -       |
| Net Sales                        | Master Linkage = 5 \| Category = Section \| Placeholder = Net Sales \| hidden = false \| disabled = true                               | Yes     |
| Increase in Net Sales            | Master Linkage = 6 \| Category = Section \| Placeholder = Increase in Net Sales \| hidden = false \| disabled = true                   | Yes     |
| Total Operating Income           | Master Linkage = 7 \| Category = Section \| Placeholder = ITotal Operating Income \| hidden = false \| disabled = true                 | Yes     |
| Trading / Other Operating Income | Master Linkage = 8 \| Category = Field \| Placeholder = - - - - Trading / Other Operating Income \| hidden = false \| disabled = false | -       |

### Excel Import Export

![](<../../.gitbook/assets/image (218).png>)

The PL BS data can be exported in excel file using this option.&#x20;

Steps:&#x20;

1. Export will give you excel file. If the screen is blank then excel file will contain template of PL BS without date
2. Then import the filled excel file in the system.&#x20;

{% hint style="warning" %}
Ensure the column headers and then first column is not altered
{% endhint %}

## **Other Details**

| **Item**                                                                                                   | **Link**                                           |
| ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------- |
| List of Fields                                                                                             | link                                               |
| List of Validations                                                                                        | link                                               |
| Masters (Dropdown + Standalone)                                                                            | link                                               |
| Possible Events                                                                                            | <ul><li>save-cam-details (pl-bs-details)</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>NA</li></ul>                               |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                                 |

### Important Link

1. For Perfios Financial Statement OCR api: [here](https://docs.google.com/spreadsheets/d/12IU69-tgLhxzjV-IUFR2OREocehCPfr11KAQj-Lp7CA/edit?usp=sharing)
2. For Karza and Probe PL BS mapping: [here](https://docs.google.com/spreadsheets/d/1Q4GHrnXOi7joPJ5Ni\_kAhscdqRRGEqZbqUhFmMLwlxc/edit?usp=sharing)

