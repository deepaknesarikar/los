---
description: Masters having records size >1000
---

# Stand Alone Masters

These masters are large masters hence saved in a separate database collection. All the masters having records size >1000 can be uploaded in the Standalone masters

{% hint style="danger" %}
Before creating any new stand alone master, Please check if that same master is  already available. If it is available, then you just need to upload the data for your institution.&#x20;
{% endhint %}

### Types of Standalone masters

Standalone masters can be of two types

1. Institute Level: These masters will be tagged to Institute. That means, you can upload only one copy of each master within one institute
2. Product Level: These masters will be tagged to each product. That means, you can upload one copy for each product within the institute   &#x20;

### Existing Standalone Masters

| No | Master Name                           | Level      | Drive Link                                                                                  | Purpose                                                                      |
| -- | ------------------------------------- | ---------- | ------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| 1  | Pincode Master                        | Institute  | [link](https://drive.google.com/file/d/1TBUGWI2ZaKO8GoWW-UUsvcJ0zTHeROnG/view?usp=sharing)  | To fetch City and State using pincode                                        |
| 2  | Company Master                        | Institute  | [link](https://drive.google.com/file/d/1zZeAwbkUDQiomm-Qubgur2AxnOhRSQCC/view?usp=sharing)  | To fetch list of company in employment details                               |
| 3  | State District Master                 | Institute  | [link](https://drive.google.com/file/d/1ipFJIMEKot-NKShHjsa9D\_tVMo-22b1F/view?usp=sharing) | To fetch District basis state                                                |
| 4  | Bank Master                           | Institute  | [link](https://drive.google.com/file/d/11-N7LH0-UrG9VaJwcWUj7jioyNBiWvmM/view?usp=sharing)  | To fetch bank name                                                           |
| 5  | IFSC Code Master (Bank Detail Master) | Institute  | [link](https://drive.google.com/file/d/1nhtM7Tx7euTvdNxm9et3E2SbMT\_Ztiym/view?usp=sharing) | To fetch bank name, branch name, MICR code using IFSC code                   |
| 6  | Deviation Master                      | Product    | [link](https://drive.google.com/file/d/16oWrJfvYA0lW2VbQLfQLD3FttH3Nh-Mo/view?usp=sharing)  | To add manual deviations                                                     |
| 7  | Deviation\_Role\_Level\_Mapping       | Product    | [link](https://drive.google.com/file/d/1SW\_2QBu80gMePBFp46DJUMPMHnoXj2hU/view?usp=sharing) | To convert sobre levels (Ex- L1/L2) into actual roles                        |
| 8  | NEGATIVE CUSTOMER DATABASE            | Institute  | [link](https://drive.google.com/file/d/1JUP2n0NgP5-NxT5Qr4HIaMmDgzapbvKb/view?usp=sharing)  | To store bad customers data and match with incoming applicants during dedupe |

{% hint style="info" %}
Pincode master will also contain Negative Area associated with that pincode.&#x20;
{% endhint %}

### Validations

Below are the validation for Standalone masters

* Records (rows in excel) should be more than 1000
* Name of the master should be unique for all standalone masters
