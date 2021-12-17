---
description: The screen can be used the pre-populate the eligibility from SoBRe
---

# Sales Eligibility

The screen can be used to data enter/ pre-populate the sobre output on the screen.&#x20;

## Description

The screen contains fields which are in below hierarchy

![](<../../.gitbook/assets/image (102).png>)

The fields at any level / or all levels can be used together to achieve the desire eligibility structure.&#x20;

![Application level](<../../.gitbook/assets/image (103).png>)

![Applicant / Program level](<../../.gitbook/assets/image (104).png>)

### Data Model

#### Application Level

```
{
      "iTenure": 0,
      "sTenureUnit": "2",
      "dApprovedAmount": 0,
      "dApprovedRoi": 0,
      "sSelectedProgram": "2",
      "sRiskCategory": "2",
      "dFoir": 0,
      "dLtv": 0,
      "dMargin": 0,
      "dGrossIncomeForApplication": 0,
      "dFixedObligationForApplication": 0,
      "oAdditionalProperties": {
        "field1": "value1",
        "field2": "value2",
        "field3": "value3",
        "field4": "value4",
        "field5": "value5",
        "field6": "value6",
        "field7": "value7",
        "field8": "value8",
        "field9": "value9"
      }
    }
```

#### Applicant Level

```
{
        "sApplicantID": null,
        "dGrossIncmeForAppl": 2500000,
        "dFixedObligationForAppl": 0,
        "dLimit": 0,
        "sBorrowerCategory": "2",
        "sRiskCategory": "2",
        "aApprovalDetails": []
}
```

#### Program Level (aApprovalDetails)

```
Same as Application Level
```

### Features

* To populate any sobre Fields in the screen, use the [Sobre-Eligibility Mapper](../../for-admins/module-level/eligibility-sobre-mapper.md)
* The extra fields can be hidden using the form config.&#x20;
* For giving multiple eligibility use the Program level fields.&#x20;
* Any field additional field is also supported at all levels
* Clicking on additional properties will open a pop-up to show the additional fields ![](<../../.gitbook/assets/image (105).png>)&#x20;

## **Other Details**

| **Item**                                                                                                   | **Link**                                   |
| ---------------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| List of Fields                                                                                             | link                                       |
| List of Validations                                                                                        | link                                       |
| Masters (Dropdown + Standalone)                                                                            | link                                       |
| Possible Events                                                                                            | <ul><li>save-eligibility-details</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>sobre-executor</li></ul>           |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                                         |
