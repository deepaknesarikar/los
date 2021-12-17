# Property Valuation

All the collaterals added in the sales screen will be pre-populated in the this screen which can used for further valuation

## Description

The screen is divided in 2 sections

* Application Details (Input)
* Valuation Report (Output)

![](<../../.gitbook/assets/image (129).png>)

### Valuation Screen

![](<../../.gitbook/assets/image (130).png>)

![](<../../.gitbook/assets/image (131).png>)

![](<../../.gitbook/assets/image (132).png>)

![](<../../.gitbook/assets/image (133).png>)

![](<../../.gitbook/assets/image (134).png>)

![](<../../.gitbook/assets/image (135).png>)

### Features

1. Multiple verification can be done for single collateral
2. Collateral details will be seen in the Input section
3. If collateral is deleted, then it will get deleted on this screen also
4. Output will be used by the roles to capture the data and upload images or documents
5. Verification Agency can be used to trigger this case to the agency. Agency type = `PROPERTY_VERIFIER`
6. Capture Geolocation Feature : [Read here](field-inspection-fi.md#capture-geolocation-feature)

{% hint style="info" %}
To link agencies to the user, please go through [Dealer master upload](../../initial-setup-product/uam-setup/upload-masters.md#type-of-agencies)
{% endhint %}

## **Other Details**

| **Item**                                                                                                   | **Link**                                                                                  |
| ---------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| List of Fields                                                                                             | link                                                                                      |
| List of Validations                                                                                        | link                                                                                      |
| Masters (Dropdown + Standalone)                                                                            | link                                                                                      |
| Possible Events                                                                                            | <ul><li>register-application</li><li>register-applicant</li><li>dedupe-executor</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>verify-PAN</li><li>SMS OTP</li><li>Email OTP </li></ul>                           |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | Yes                                                                                       |
