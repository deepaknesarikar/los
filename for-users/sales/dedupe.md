---
description: View the dedupe output result
---

# Dedupe

The screen can be used to&#x20;

* view dedupe results
* re-trigger dedupe
* Pre-populate one the  Dedupe result in the demographic screen
* Mark match / no-match against the dedupe output record

## Description

Dedupe can be triggerred from&#x20;

* Sourcing screen for the contact person details
* Demographic screen for each Applicant added
* From the Dedupe screen for one or multiple applicant

![](<../../.gitbook/assets/image (226).png>)

### Dedupe Flow

![](<../../.gitbook/assets/image (106).png>)

The output of the dedupe will be shown on the Dedupe screen. The same screen can be used to pre-populate the output data in any one the applicant or even create new applicant

{% hint style="info" %}
The Dedupe screen can be seen in pop-up from the Sourcing and Demographic screen as well.&#x20;
{% endhint %}

## Negative Customer Database

All the existing customer can be migrated into a master and stored there for dedupe purposes. The data has to uploaded in the below format.&#x20;

You can download the master from[ Standalone Masters](../../for-admins/masters/untitled-2.md)

Note: More the data, the dedupe API will be executed slowly

## Available Dedupe Logic

| NAME                                                                    | DESC                                                                                                                                     |
| ----------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Match only KYCs                                                         | <p>Will match all KYC inputted in the case</p><p>Individual: Pan, Passport, Voter, DL, Aadhar</p><p>Non-Individual: CIN , GST, Udyam</p> |
| Match KYC + Mobile no                                                   | All above KYC AND mobile                                                                                                                 |
| Match KYC + Mobile + Email ID                                           | All above AND email                                                                                                                      |
| Match KYC + Mobile + Email + Address                                    | All above AND Address (line1, line2, pincode, city, state)                                                                               |
| Match First and Last name + KYC                                         | Above KYC AND firstname AND last name                                                                                                    |
| Match First and Last name + KYC + Mobile + Email + DOB                  |                                                                                                                                          |
| Match First and Last name + KYC + Mobile + Email + DOB+ Address         |                                                                                                                                          |
| Match KYC or Mobile or Name+DOB+ApplicantType or Name+DOI+ApplicantType |                                                                                                                                          |
| HDB Dedupe                                                              | Details are present in this jira: [https://lentra.atlassian.net/browse/CAM-662](https://lentra.atlassian.net/browse/CAM-662)             |

## **Other Details**

| **Item**                                                                                                   | **Link**                                                      |
| ---------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| List of Fields                                                                                             | link                                                          |
| List of Validations                                                                                        | link                                                          |
| Masters (Dropdown + Standalone)                                                                            | link                                                          |
| Possible Events                                                                                            | <ul><li>save-dedupe-details</li><li>dedupe-executor</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>NA</li></ul>                                          |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                                            |
