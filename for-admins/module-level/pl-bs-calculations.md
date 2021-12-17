---
description: Add PL BS calculations from the UI
---

# Calculations Config

The screen will be used to input the  below type of calculations (formula)&#x20;

* ProfitLoss and BalanceSheet
* Ratio Analysis
* Cashflow Analysis

**For a single product, user can 3 types of Calculation Types.**&#x20;

1. One for Cashflow
2. One for Ratio Analysis
3. Two for PL and BS. Inside PL and BS, you can have one for Profit Loss and one for BalanceSheet&#x20;

## Add Calculations

1. Click on "Create Calculation" button

![](<../../.gitbook/assets/image (70).png>)

2\. Select the fields as per the form

3\. Keep on adding formulas for the selected type of calculation

{% hint style="info" %}
Multiple Fields can be added in each type. For example, the you can calculate 15 ratios using the calculationType = Ratio
{% endhint %}

### Type: CASHFLOW

![](<../../.gitbook/assets/image (71).png>)

| Field Name    | Description                                                                                                                                     |
| ------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Products      | Select the appropriate Product                                                                                                                  |
| Field Name    | Enter the field name. This will be used as backend Field                                                                                        |
| Display Name  | Enter the field name. This will be shown on the Screen                                                                                          |
| Priority      | The priority determines the sequence (starting from 1) of the formula execution. Ex - If 1 is entered, then that formula will be executed first |
| Formula       | Enter the formula. Details [here](pl-bs-calculations.md#how-to-create-a-formula)                                                                |

### Type: RATIO

![](<../../.gitbook/assets/image (72).png>)

| Field Name       | Description                                                                                                                                     |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Calculation Name | Ratios can be grouped together with a name. Enter the group name which will should on the UI                                                    |
| Products         | Select the appropriate Product                                                                                                                  |
| Field Name       | Enter the field name. This will be used as backend Field                                                                                        |
| Display Name     | Enter the field name. This will be shown on the Screen                                                                                          |
| Priority         | The priority determines the sequence (starting from 1) of the formula execution. Ex - If 1 is entered, then that formula will be executed first |
| Formula          | Enter the formula. Details [here](pl-bs-calculations.md#how-to-create-a-formula)                                                                |

### Type: PL AND BS

|   |
| - |

![](<../../.gitbook/assets/image (73).png>)

| Field Name       | Description                                                                                                                                                                                                                                                      |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Calculation Name | <p>Select the formulas which you want to set. Either <strong>ProfitLoss</strong> or <strong>BalanceSheet</strong></p><p><strong></strong></p>                                                                                                                    |
| Products         | Select the appropriate Product                                                                                                                                                                                                                                   |
| Field Name       | Enter the field name. This will be used as backend Field                                                                                                                                                                                                         |
| Display Name     | <p>This field is a dropdown. It should fields where the values have to set. <em>Basically, this field is where your formula output will be stored.</em>  </p><p><em></em><span data-gb-custom-inline data-tag="emoji" data-code="1f4a1">💡</span> <em></em> </p> |
| Priority         | The priority determines the sequence (starting from 1) of the formula execution. Ex - If 1 is entered, then that formula will be executed first                                                                                                                  |
| Formula          | Enter the formula. Details [here](pl-bs-calculations.md#how-to-create-a-formula)                                                                                                                                                                                 |

## How to create a formula

Entering formula is easy. You have to select the fields to be used in the formula and add operators to it.

#### Step1:&#x20;

Click on the formula input field which will open a pop-up like below. You can use the **"+"** button to add one more variable

![](<../../.gitbook/assets/image (77).png>)

#### Step2:

Select the dropdown to choose the operator or directly a field from dropdown. Type in Search box to search for specific field.&#x20;

![Fields List](<../../.gitbook/assets/image (75).png>)

![Operators : Add \[+\] , Subtract \[-\] , Multiply \[\*\] , Divide \[/\] , Parentheses \[ ( ) \] ](<../../.gitbook/assets/image (74).png>)

#### Step3:

The below image shows formula entered

$$
( PL CostOfGoodsSold * PL AdminExpenses ) / PL GrossProfits
$$

Click on Save one done&#x20;

![](<../../.gitbook/assets/image (76).png>)



{% hint style="info" %}
If you entering the formula for either for ProfitLoss or BalanceSheet then the respective fields will only come in the dropdown.&#x20;

Ex - For Calculation Type Name = ProfitLoss; only fields on profit loss will come in the dropdown
{% endhint %}
