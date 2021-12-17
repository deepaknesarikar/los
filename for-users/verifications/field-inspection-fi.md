---
description: Perform CPV / FI for your customer addresses
---

# Field Inspection (FI)

This screen will be useful for address verification agencies to visit and record the observations for each address.&#x20;

## Description

The screen is divided into applicant address level. That means, the verification report can be filled for each address. &#x20;

![](<../../.gitbook/assets/image (136).png>)

### Verification Screen

![](<../../.gitbook/assets/image (137).png>)

![](<../../.gitbook/assets/image (138).png>)

### Features

1. The list of address will come from the demographic screen.&#x20;
2. The address details will get updated at each save of the demographic screen.&#x20;
3. Verification report can be filled by the agency. Agency Type = `FIELD_VERIFIER`

{% hint style="danger" %}
The Address gets updated at each demographic save. Hence it should be ensured that once the FI work has started, demographic screen data should **not** be allowed to get updated or saved.&#x20;
{% endhint %}

#### Capture Geolocation Feature

This will help you to capture the goelocation using laption / mobile and store it in the map. This feature does not require Google API is is available free.&#x20;

| Before Capture                                | After Capture                                 |
| --------------------------------------------- | --------------------------------------------- |
| ![](<../../.gitbook/assets/image (192).png>)  | ![](<../../.gitbook/assets/image (193).png>)  |

### Calculate Geolocation distance from branch

This feature is developed in GNG to capture the distance between Customer Location(FI & PD screen) and Branch(Selected on sourcing screen) with the help of Lat-Long.

{% hint style="info" %}
To capture Geo-location please ensure that you have allowed browser location access permission. Refer image below
{% endhint %}

![](https://lh3.googleusercontent.com/vZAfuLStI06om9sfSpsHitpJIjtEhObUDMX-12hdTR4M8cFo-OJ3EuT7ElscFdt-rzbmuRG2C1S4StUmt\_s0771hyuyc\_yb26KQcPdKjnCMlK\_PmstTTrJktkRapIsOOI2wjqmw9=s1600)

Step 1:  Upload the branch Lat-Long on UAM - [Branch Pool Master](../../initial-setup-product/uam-setup/upload-masters.md). You need to add two columns in the master

![](https://mail.google.com/mail/u/1?ui=2\&ik=68236c0459\&attid=0.0.2\&permmsgid=msg-f:1714144452998961831\&th=17c9dd4c4eb59aa7\&view=fimg\&fur=ip\&sz=s0-l75-ft\&attbid=ANGjdJ8Yvcw7g9EIC1bPOtM0D0nUYMMnFocJPTpwH-AFL43gnq6P-j9M9s3F4TYCzc7LWf7Ja9IHJMdZGQ5jmSK9aziyE8bd67ASmOzWy0jILKg6mlEb9OoqmOKB9b8\&disp=emb\&realattid=ii\_kuzj6fcu2)

* LATITUDE
* LONGITUTE

Step 2: Branch Selection on Sourcing Screen

![](https://mail.google.com/mail/u/1?ui=2\&ik=68236c0459\&attid=0.0.1\&permmsgid=msg-f:1714144452998961831\&th=17c9dd4c4eb59aa7\&view=fimg\&fur=ip\&sz=s0-l75-ft\&attbid=ANGjdJ8qbnmDvyiZqLeuIXTykwf5ns1VC-NGyKrvJmqIx-98lLuPWe4IcAeXFQMA4bihVnwgCVNAWrkbg23n-v8sU5\_9xru4qXK-hapJrUxgpyMjgLsmcIEIeUV7AEs\&disp=emb\&realattid=ii\_kuzj279v1)

Step 3: Once the master is uploaded with Branch Lat-Long details and Location access is granted you can check the distance between branch Lat-Long and User Lat-Long.

![](https://mail.google.com/mail/u/1?ui=2\&ik=68236c0459\&attid=0.0.3\&permmsgid=msg-f:1714144452998961831\&th=17c9dd4c4eb59aa7\&view=fimg\&fur=ip\&sz=s0-l75-ft\&attbid=ANGjdJ8ChMvWPk1G0Z4hq\_T-15RqFpWj0eboSym02xBTJoJmvdoE\_lg7enYCQCCAMhOkEMV1KIK6dT7Fu2ya0VefukBjFTOyRNZSzpZXR\_P5NuJ-pAZxfUxNSzVHtic\&disp=emb\&realattid=ii\_kuzj9zhr3)

\
\
Check the distance between customer Lat-Long and Branch on FI and PD screen by capturing the customers Lat-Long

**This will fetch the user the aerial distance between the Branch and User location.**\
Note: This feature is currently implemented on FI and PD screens only

## **Other Details**

| **Item**                                                                                                   | **Link**                                  |
| ---------------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| List of Fields                                                                                             | link                                      |
| List of Validations                                                                                        | link                                      |
| Masters (Dropdown + Standalone)                                                                            | link                                      |
| Possible Events                                                                                            | <ul><li>save-field-verification</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>NA</li></ul>                      |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | Yes                                       |
