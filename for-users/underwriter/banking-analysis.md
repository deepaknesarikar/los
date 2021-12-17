---
description: View bank statement analysis
---

# Banking Analysis

This screen will help user to view the pre-populated data from the Bank-statement-analyzers apis or even do a data entry of the analysis. Basis the input values, the screen will calculate the summary, total and average fields.

## Description

The screen is divided into 4 sections. All the sections are available for each applicant

1. Summary (At Application level which is aggregation level)
2. Basic details (at bank statement level)
3. Monthly Details (at bank statement level)
4. Other Details (at bank statement level)

### Summary

These values are calculated by aggregating all the input values of all the bank statements.&#x20;

![](<../../.gitbook/assets/image (116).png>)

### Basic Details Section

This section will contain basic details of the bank accounts

![](<../../.gitbook/assets/image (117).png>)

### Monthly Details

This section will help user to capture / view the monthly details. The fields and their types area as follow&#x20;

![](<../../.gitbook/assets/image (118).png>)

| Field name            | Desc                                  |
| --------------------- | ------------------------------------- |
| Month                 | Input / Pre-populated                 |
| Date wise balances    | 5/ 10 / 15/ 20/ 25                    |
| ABB                   | Average of the date wise balances     |
| Limit                 | Input                                 |
| Outflow (debit)       | Summation / Substraction can be added |
| Inflow (credit)       | Summation / Substraction can be added |
| Net Flow              | Outflow - Inflow                      |
| Cash Withdrawals      | Input                                 |
| Cash Deposits         | Input                                 |
| Withdrawals / deposit | Withdrawals / Deposits (divided by)   |
| Peak utilization      | Input                                 |
| Over utlization       | Input                                 |
| Interest Debited      | Input                                 |
| Inward Returns        | Input                                 |
| Outwards returns      | Input                                 |
| Credit Entries        | Count                                 |
| Debit entries         | Count                                 |

#### Monthly Summary

* Total of all the above fields
* Average of all the above fields
* No of Credit / Debit transactions
* Inward bounce %
* Outward bounce %

## Other Details

![](<../../.gitbook/assets/image (119).png>)

## **Other Details**

| **Item**                                                                                                   | **Link**                                              |
| ---------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| List of Fields                                                                                             | link                                                  |
| List of Validations                                                                                        | link                                                  |
| Masters (Dropdown + Standalone)                                                                            | link                                                  |
| Possible Events                                                                                            | <ul><li>save-cam-details (banking-analysis)</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>NA</li></ul>                                  |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                                    |
