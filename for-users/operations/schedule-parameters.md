---
description: Capture repayment schedule parameters and generate schedule
---

# Schedule Parameters

The screen will help users to capture the Schedule parameters

## Description

![](<../../.gitbook/assets/image (142).png>)

#### Features

Capture Schedule parameteres which are as below

| Field                       | Logic                                                                                                                                       |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Expected Disbursement Date  | Current Date is set                                                                                                                         |
| Cycle Day                   | Dropdown master with due date as value                                                                                                      |
| Installment Start Date      | Next Cycle day is used by adding 30 days                                                                                                    |
| BPI date                    | User Input                                                                                                                                  |
| Repayment Variation         | Master ( Regular / stepped / Advance EMI)                                                                                                   |
| Loan Amount                 | Auto-populated from the Credit Eligibility                                                                                                  |
| ROI                         | Auto-populated from the Credit Eligibility                                                                                                  |
| Tenure                      | Auto-populated from the Credit Eligibility                                                                                                  |
| No. of Installments         | Monthly / Querterly / Half-yearly / Yearly                                                                                                  |
| Repayment Frequency         | <p>If monthly then Tenure /  12</p><p>If quarterly then Tenure / 4</p><p>If half-yearly then Tenure / 2</p><p>If yearly then Tenure / 1</p> |
| BPI calculation Method      | Dropdown (Actual/Actual or Actual/360)                                                                                                      |
| Interest Calculation Method | Dropdown (Actual/Actual or Actual/360)                                                                                                      |
| Interest Rate Type          | Fixed / Floating                                                                                                                            |
| EMI                         | Calculated as the PMT formula                                                                                                               |
| Advance EMI                 | <p>Only if Repayment Variation = advance</p><p>Integer Input</p>                                                                            |
| Step Type                   | <p>Only if Repayment Variation = stepped</p><p>(Step up / Step down / Absolute)</p>                                                         |

#### Stepped Schedule

![](<../../.gitbook/assets/image (143).png>)

This can be inputted if the schedule is structured in nature.&#x20;

## **Other Details**

| **Item**                                                                                                   | **Link**                                  |
| ---------------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| List of Fields                                                                                             | link                                      |
| List of Validations                                                                                        | link                                      |
| Masters (Dropdown + Standalone)                                                                            | link                                      |
| Possible Events                                                                                            | <ul><li>save-repayment-schedule</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>LentraLMS API</li></ul>           |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                        |
