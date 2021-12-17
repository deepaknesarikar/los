---
description: Enter Tranche and Payment request details
---

# Disbursement Memo

The screen will be used to enter the request details for transfering the payments to the borrowers

## Description

The screen is divided in 2 sections

* Summary
* Request Details

### Disb Summary

![Disbursement Summary](<../../.gitbook/assets/image (144).png>)

The summary calculations are auto-calculated and formula are as below

Net Disbursement Amount = `Approved Amount - Amount Financed + Amount Deducted`

Amount Disbursed = `Sum of Disbursement Amount from Request Details where payment is Completed`

Amount Cancel = `Sum Sum of Disbursement Amount from Request Details where payment is Cancelled`

Undisburse Amount = `Net Disbursement Amount - Amount Disbursed - Amount Cancel`

### Request Details

![Disbursement Request Details](<../../.gitbook/assets/image (145).png>)

All the payment details can be entered on this screen. The purpose of the screen is for

* Disbursement Payment (credit and debit both) details.&#x20;
* Multiple Tranche details and their beneficiary details
* Split Disbursement (One tranche but paid to multiple beneficiary)

The Request details have below information

* Tranche No: Auto incremented from 1
* Disbursement Date: Can be current or future date
* Disbursement Amount: Integer. Has to be less than Un disbursed Amount

#### Benefiary Details

![Request Beneficiary Details](<../../.gitbook/assets/image (146).png>)

The screen is used to capture the beneficiary (creditors) details and the debit account details

### Flow of Payment

![](<../../.gitbook/assets/image (147).png>)

{% hint style="info" %}
For any Disbursement Memo and related documents please use the [Templates](../others/templates.md) to configure the documents
{% endhint %}

## **Other Details**

| **Item**                                                                                                   | **Link**                                                                       |
| ---------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| List of Fields                                                                                             | link                                                                           |
| List of Validations                                                                                        | link                                                                           |
| Masters (Dropdown + Standalone)                                                                            | link                                                                           |
| Possible Events                                                                                            | <ul><li>save-disb-memo</li></ul>                                               |
| 3PI APIs                                                                                                   | <ul><li>Payment API of Client</li><li>Customer / Loan booking in LMS</li></ul> |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                                                             |
