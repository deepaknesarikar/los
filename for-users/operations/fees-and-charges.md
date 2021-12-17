---
description: Capture and calculate the fees / charges and Insurances
---

# Fees and Charges

The screen contains 3 sections

1. Fees: Fees which are collected before or at the time of disbursement
2. Charges: Fees which are collected after the disbursement. Mainly in LMS
3. Insurance: Insurance which are associated with Application / Collateral / Applicant

## Description

### Section1: Fees

#### Features

* The screen uses feesCharge [master](fees-and-charges.md#fees-charge-master)
* Mandatory fees will be auto-populated on the screen
* The calculation method can be Forward and Reverse
  * Forward = Calculation starts from Percentage of Fees amount and then Tax and "Net recievable" is calculated
  * Reverse = Calculation starts from "Net Recievable" and then the Fees / Tax is calculated
* Deposit details pop-up contains the Credit and Debit details of the fees.&#x20;
* Fees can be paid via more than one way. Ex - If fees is 100/- then 50 can be paid in cash and 50 via Cheque. both the details can be tracked in the Deposit Details Pop-up
* The Recovery mode can be&#x20;
  * Initial Reciept: Will be paid by customer upfront
  * Deduct From Disb: will be deducted from the disbursement amount
  * Financed: Will be Financed and added to disbursement amount

![Fees Table](<../../.gitbook/assets/image (154).png>)

![Fees Summary](<../../.gitbook/assets/image (155).png>)

#### Formulas for the fees fields

| Field          | Possible Formula                                         |
| -------------- | -------------------------------------------------------- |
| Fee %          | Input / can come from master                             |
| Fees Amount    | Input / can come from master / Fees % \* Approved Amount |
| Tax Amount     | Fees Amount \* (Tax from master /100)                    |
| TDS %          | Input                                                    |
| TDS Amount     | Fees Amount \* (TDS%  /100)                              |
| Net Recievable | Fees Amount + Tax Amount - TDS Amount                    |

Formulas for Summary fields

![Deposit Details Pop-up](<../../.gitbook/assets/image (158).png>)

### Section2 : Charges

Charges are added on this screen which are to be passed on to the LMS

![Charges table](<../../.gitbook/assets/image (156).png>)

If the Charge Type = Range, then the Range pop-up can be used for entering the range wise charges

* Range has to be in no. of tenor
* Repaid Principle Has to be entered in %
* Amount or Amount % can be entered

![If Charge is Range, then enter range details](<../../.gitbook/assets/image (159).png>)

### Section3: Insurance

* Insurance details can be entered in this section
* Formulas in summary are
  * Total Net Premium = `Gross Premium + Total GST`
  * Total GST = `Gross Premium * 18%`

![](<../../.gitbook/assets/image (157).png>)

### Fees Charge Master

* The columns which are marked in Yellow are mandatory for Gonogo.&#x20;
* The description of the columns are mentioned in the 2nd row. Rest rows contain the sample values
* Link of the Fees master: [feesChargeMaster](https://drive.google.com/file/d/1Ms8Tr9RXZxTECmIQ3mPZmQrzesbLNfzT/view?usp=sharing)&#x20;

{% hint style="info" %}
sChargeCode is to be used for Integration

sFeeType is used on the UI
{% endhint %}

## **Other Details**

| **Item**                                                                                                   | **Link**                            |
| ---------------------------------------------------------------------------------------------------------- | ----------------------------------- |
| List of Fields                                                                                             | link                                |
| List of Validations                                                                                        | link                                |
| Masters (Dropdown + Standalone)                                                                            | link                                |
| Possible Events                                                                                            | <ul><li>save-loan-charges</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>NA</li></ul>                |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                  |
