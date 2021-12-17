---
description: Analyse the repayment history of the applicants
---

# Repayment Track Record

The screen will help users to view the existing active loans of the applicant and enter / update the data of the loans

## Description

The screen is divided into 3 sections out of which first section is the important one.&#x20;

### Features

* This screen is applicant wise. I.e. for each applicant you can fill all the below 3 sections
* The data filled here is available in sobre for writing rules
* All the extra fields can be hidden using the form config

### Section1: RTR

![Summary of Repayment Details](<../../.gitbook/assets/image (108).png>)

![Details of Single Loan](<../../.gitbook/assets/image (109).png>)

Here the data can come from two sources

* Merge report of the MB
* Data entry by the users

#### Summary Description

|                                                 |                                                      |
| ----------------------------------------------- | ---------------------------------------------------- |
| Total EMI(₹) :-                                 | Sum of all EMI of all the loans                      |
| Obligation Not Considered For Eligibility(₹) :- | Sum of EMI of the loans which are marked as FO = No  |
| Net Fixed Obligation(₹) :-                      | Sum of EMI of the loans which are marked as FO = Yes |
| "OE" Operating FO (TL / CC / OD) :-             |                                                      |
| Net Fixed Obligation(₹) :-                      |                                                      |

### Section2: Facility Details

![](<../../.gitbook/assets/image (111).png>)

### Section3: Loan Details

### &#x20;

![](<../../.gitbook/assets/image (112).png>)



## **Other Details**

| **Item**                                                                                                   | **Link**                                         |
| ---------------------------------------------------------------------------------------------------------- | ------------------------------------------------ |
| List of Fields                                                                                             | link                                             |
| List of Validations                                                                                        | link                                             |
| Masters (Dropdown + Standalone)                                                                            | link                                             |
| Possible Events                                                                                            | <ul><li>save-cam-details (rtr-details)</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>NA</li></ul>                             |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                               |
