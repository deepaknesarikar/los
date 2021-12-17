---
description: Scan all uploaded documents for Fraud
---

# RCU

RCU (risk control unit) will help the users to scan and analyze documents for any discrepencies and fraud and then mark them as sampled or Screened.&#x20;

## Description

The screen is divided into below sections and the flow of documents is as below.&#x20;

#### Flow of a document

All the documents are scanned and they form the funnel. The Sample funnel / flow of the document through RIC screen is shown below

![](<../../.gitbook/assets/Screenshot from 2021-03-23 11-44-56.png>)

### Section1: RCU Summary

![](<../../.gitbook/assets/image (160).png>)

* This section shows you summary of all the documents in different statuses. It will be helpful for user to get a overview of the case
* On the right, Agency can be triggered using the dropdown of agencies.&#x20;
* Fraud report will show a hunter report to the RCU user. Read through this document to know more about [hunter integration](https://docs.google.com/document/d/1DTff4kR1s\_NxbIMXdEO0Pvr0JXn\_j2n9OoTK-dVy4uI/edit?usp=sharing)

### Section2: Mark for RCU &#x20;

![](<../../.gitbook/assets/image (161).png>)

* This sections shows **all** the document which have been uploaded in the case.
* User can then select the document for RCU process out of the all the documents. As per the selected, the summary count of "Documents selected for RCU will change".&#x20;
* All the selected documents are shown in Green button

### Section3: Screener / Sampler Section

![](<../../.gitbook/assets/image (162).png>)

* All the documents which are marked as RCU will come to this table
* User can then click on the record to open the image.&#x20;
* User has to input below fields
  * RCU Status: It can be screened / sampled / pending
  * Document Remarks (Optional)
  * Verification Status (Master = rcuDecision)&#x20;
  * RCU Remarks
* Same can also be done on the image pop-up
* User gets Next / Previous button so that he can navigate between the images easily

![View Image Pop-up](<../../.gitbook/assets/image (163).png>)

### Section4: Authoriser Section

* After Screening and Sampling is done, RCU authority can give a final decision on the case.
* Remarks can be entered for justifying the decision
* Any documents or reports can also be uploaded here.

![](<../../.gitbook/assets/image (164).png>)

## **Other Details**

| **Item**                                                                                                   | **Link**                   |
| ---------------------------------------------------------------------------------------------------------- | -------------------------- |
| List of Fields                                                                                             | link                       |
| List of Validations                                                                                        | link                       |
| Masters (Dropdown + Standalone)                                                                            | link                       |
| Possible Events                                                                                            | <ul><li>save-rcu</li></ul> |
| 3PI APIs                                                                                                   | <ul><li>Hunter</li></ul>   |
| [Custom Object](../../for-admins/product-level/custom-objects.md#process-to-create-custom-objects) Support | No                         |
