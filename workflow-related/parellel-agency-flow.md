---
description: >-
  Allow two users to work parellel on the same application (but on different
  screens)
---

# Parellel Flow

### Introduction

Agency Flow will be required if the two roles have to work simultanously on the same case **but on different screens**. This would require special configurations which are mentioned in this page. There can be two ways to configure the parellel flow which is mentioned below

|                 | Parellel Flow for Agency                                                                                                      | Parellel for Role                                         |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------- |
| Intro           | Should be used if the task is outsourced to some agency and then internal user is going to trigger to the respective agency.  | Should be used if two roles who are in-house want to work |
| Allocation      | Allocation basis Dealer ID + Agency Status + Role                                                                             | Allocation basis stage + Branch hierarchy + Role          |
| Trigger         | Manual Trigger                                                                                                                | Automatic Trigger                                         |
|                 | Agency and Role wise allocation                                                                                               | Only Role wise allocation                                 |
| Config required | Dashboard config + Action Config + Form Config                                                                                | Workflow + Dashboard config + Action Config + Form Config |

## Parellel Flow for Agency

Step1: Upload [Dealer Master ](../initial-setup-product/uam-setup/upload-masters.md)in UAM with appropriate [Verification Type](../initial-setup-product/uam-setup/upload-masters.md#type-of-agencies). The verification&#x20;

Step2: The person who is going to select the agency, should be assigned all the agencies to whom he can assign. This has to be done in UAM in [Users](../initial-setup-product/uam-setup/create-users.md#dealer-master)

Step3: The agency users has to be assigned with the respective agency. **Note: Agency users can only have one Dealer**

Step4: After login, you will get the agencies in the dropdown of the triggering user.&#x20;



## Parellel for Role

Require to upload the dealer master in the UAM. The verification Type column should have value of the respective screen. Gonogo, has auto-lock feature which locks the case once any user picks it up. So the next user who is picking the case will get the case read-only
