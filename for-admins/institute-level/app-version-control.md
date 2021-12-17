---
description: Allow the latest Client version to access the backend
---

# App Version Control

This module can be used to whitelist only the correct and bug-free UI (Web + Andriod) version on the backend. This will automatically stop all the API hits coming from the non-whitelisted versions

Example - In the below image "Andriod: 1.09.01 UAT" is the version whitelisted. Hence this version users will be able to access the backend APIs

![](<../../.gitbook/assets/image (21).png>)

### How to add versions

For Web: Follow this pattern "WEB" + " " + "Version". `Example - WEB 2.12.02`

For Andriod: Follow this pattern "Andriod" + ":" + "Version". `Example -`` `_`Android:1.09.01 UAT`_

{% hint style="danger" %}
Error seen at the time of login case of wrong App Version added is below

"You are using unsupported version of the app"
{% endhint %}
