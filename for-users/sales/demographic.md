---
description: Screen for capture Applicants information
---

# Demographic

This screen will be helpful to capture the applicant information (both individual and non-individual).&#x20;

## Description

![](<../../.gitbook/assets/image (94).png>)

### Features

This screen is used to enter the details of all the applicants (parties to the loan). You can add multiple applicants to the loan depending on the policy. The constitution of the Applicant can be as below

* Individual
* Non-Individual
  * Company
  * Proprietorship
  * Partnership
  * LLP
  * HUF
  * AOF (Associations of Persons)

Depending on the constitution of the applicant, relevant fields will be displayed on the screen.

#### Sections

| Sections               | Applicable for              |
| ---------------------- | --------------------------- |
| Business Details       | All Non-Individual          |
| Address                | Individual + Non-Individual |
| References             | Individual + Non-Individual |
| Contact Person Details | Individual + Non-Individual |
| MCA Signatories        | Only Company                |
| KYC Details            | Individual + Non-Individual |
| Employment Details     | Individual                  |

#### Type of Applicants

* PRIMARY: Main applicant of the case
* CO\_APPLICANT: All parties to the loans which are co-applicants
* GUARANTOR: Gaurantor to the loan
* SELLER:  Seller of the collateral in case of mortgage loans
* POA: Power of attorney - person who has legal rights to mortgage property but real owner is different. <mark style="color:blue;">Multibureau is not triggered for POA type of applicant</mark>

{% hint style="info" %}
The type of Applicant can be selected in the below dropdown

![](<../../.gitbook/assets/image (258).png>)
{% endhint %}

#### API usage for Pre-population of Data

| API name           | Use                                          |
| ------------------ | -------------------------------------------- |
| CIN                | Business Details + Address + MCA Signatories |
| PAN                | Business Name / Individual Name              |
| Driving License    | Address                                      |
| Passport           | Address                                      |
| Electricity Bill   | Address                                      |
| Voter              | Individual Name + Address                    |
| LPG Bill           | Address                                      |
| GST                | Business Details + Address                   |
| Udyam Registration | Businesss details + Address + Bank Account   |

## **Other Details**

| **Item**                                                                                                   | **Link**                                                                                                                                                                                                                                                                         |
| ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| List of Fields                                                                                             | link                                                                                                                                                                                                                                                                             |
| List of Validations                                                                                        | link                                                                                                                                                                                                                                                                             |
| Masters (Dropdown + Standalone)                                                                            | link                                                                                                                                                                                                                                                                             |
| Action Name                                                                                                | CL-DEMOGRAPHIC + CASE\_LOGIN                                                                                                                                                                                                                                                     |
| Possible Events                                                                                            | <ul><li>save-demographic</li><li>MultiBureau-executor</li><li>Sobre-executor</li><li>Dedupe-executors</li></ul>                                                                                                                                                                  |
| 3PI APIs                                                                                                   | <ul><li>verify PAN</li><li>verify Voter</li><li>verify Driving License</li><li>Search CIN by company Name</li><li>verify CIN</li><li>verify Passport</li><li>SMS OTP</li><li>Email OTP</li><li>Hunter Fraud check</li><li>verify electricity bill</li><li>verify lpg</li></ul>   |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | <p>Yes : <mark style="background-color:orange;">Custom object can be linked even basis constitution types.</mark> </p><p>Applicant: Will show for all constitution </p><p>Individual: Will show for only Individual</p><p>NonIndividual: Will show for all except Individual</p> |
