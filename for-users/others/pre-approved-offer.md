---
description: A pop-up comes in case of pre-approved offer is present
---

# Pre-Approved Offer

### Purpose

If in the loan application journey, the applicant has any pre-approved offer present then that can be shown in this pop-up. The offer can come from

* External client API
* BRE (Sobre)

### Description

The pop-up has 60 sec timer. That means the pop-up will wait for 60 sec till the offer comes.&#x20;

* If the offer comes, then approve or decline buttons are shown
* If offer doesnt come in 60 sec, then close button is shown, which will take user to the next screen

![](<../../.gitbook/assets/image (248).png>)

The pop-up has below fields

* Tenure : Tenure present in the offer. _If not present then will be shown as NA_
* ROI : Rate of interest in %. _If not present then will be shown as NA_
* EMI: EMI present in the offer. _If it is not present, then it will get calculated on the UI provided Tenure and ROI are present_
* Offer Amount : The amount will be displayed here
  * Default, the cursor will be at max. I.e. user cannot select anything more than the offer amount
  * The minimum amount is shown at 50% of the offer amount
  * User can slide the cursor or enter the required offer amount to change it

### How to configure

The offer pop-up can be shown on the "Next" button of below screens

1. Sourcing
2. Demographic
3. Financial

Each of this screen will have the below property. That property has to be added for the respective screen and the value of it should be marked as `true`

**Property Name** : showOfferPopupOnNextClick

![](<../../.gitbook/assets/image (249).png>)

## Behaviour

Once the offer is shown, user can click Approve or Decline. Each of these buttons have workflow event attached to it.&#x20;

* Approve : Event name = offer-Accept
* Decline: Event name = offer-Decline

You can decide to change the stage / status on this events. Both the events will be available in workflow module
