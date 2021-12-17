---
description: See templates and reports
---

# Templates and E-sign

Templates screen will help you to generate and view the templates which are configured for the users.&#x20;

![](<../../.gitbook/assets/image (85).png>)

### Description

1. Name of the templates selected
2. Search box for templates
3. List of Templates eligible for the Role / Stage
4. Print / Download button to print or download as pdf

The templates shown here are of two types. Refer [Template config](../../for-admins/module-level/templates.md) for mroe details

* Document
* Custom\_Document

{% hint style="danger" %}
If no templates are visible, then check if access is given to the user's **role, Product** and **Stage** in the [templates](../../for-admins/module-level/templates.md) configuration
{% endhint %}

## E Sign

![](https://lh5.googleusercontent.com/udzJxApg4Iu4rR0xNYAs1DnAKiPAz7vAAryBBHC9kv-iE6SNItT11cXBPzXIOSUjMLdoJQkoXydu3KxSkD6zLivHfy2L1mjpkLO4oXAdxFT2L5MhlcR4m1RfuzF5nUZ-hqZjxOmo=s0)

All the templates which are marked as E-sign configs are loaded here for e-sign.&#x20;

The stages of e-sign are as below

1. Document generation in progress: PDF is getting generated for esigning
2. Trigger E-sign:  Document is ready for trigger
3. Pending for Sign: Document has been triggered and pending for esign by applicant
4. E-sign Done: E-sign is successfully done
5. Error: Error in case of failure to e-sign

#### Most common errors

1. LOD document missing: If any of the document marked in Admin configis not present in the case, then it will show error that document is missing
2. Template missing: Any of the template marked for e-sign is missing then that template name will be shown as erro
3. HubX service down: If hubx e-sign service is down.&#x20;

