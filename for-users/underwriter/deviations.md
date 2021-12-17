---
description: Raise, view and approve deviations
---

# Deviations

Use this screen to raise deviations and then get them approved by the appropriate authority&#x20;

## Description

The deviations can be raised by using the "+Add" button or they can come from sobre also

![](<../../.gitbook/assets/image (120).png>)

### Raising Deviations Manually

Deviations master ([link](https://drive.google.com/file/d/16oWrJfvYA0lW2VbQLfQLD3FttH3Nh-Mo/view?usp=sharing)) should be updated at product level in order to get the list of deviations for adding them manually.&#x20;

The description of the master fields is below

* DEVIATION ID: Incremental number from 1
* DEVIATION: Deviation Description
* CATEGORY: Category&#x9;
* AUTHORITY: List of Roles to which the deviation should be raised. It can be _multiple_
* LEVEL: Levels (ex - L1, L2). Only one
* MITIGATION: Not used
* SEVERITY: Ex - S1, S1

![](<../../.gitbook/assets/image (121).png>)

### Auto-Deviations

Auto-deviations will come from sobre and can be pre-populated directly in the deviation screen.&#x20;

Pre-requisite for Auto-deviations to work

* [ ] Deviations should be configured in Sobre
* [ ] Deviation to role mapping master ([link](https://drive.google.com/file/d/1SW\_2QBu80gMePBFp46DJUMPMHnoXj2hU/view?usp=sharing)) should be uploaded for the product. The Level in the sobre deviation and the master should be in-sync
* [ ] Sobre-Deviation profile should be enabled

![](<../../.gitbook/assets/image (122).png>)

### Deviations Movement

Once the deviations are raised, the case can be submitted to the appropriate authority by selecting the role from the dropdown. User can click on submit button and the case will be move the authority dashboard.&#x20;



## **Other Details**

| **Item**                                                                                                   | **Link**                                                          |
| ---------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| List of Fields                                                                                             | link                                                              |
| List of Validations                                                                                        | link                                                              |
| Masters (Dropdown + Standalone)                                                                            | link                                                              |
| Possible Events                                                                                            | <ul><li>save -deviation-matrix</li><li>sobre-executorv2</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>NA</li></ul>                                              |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                                                |
