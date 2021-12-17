# Lock Unlock

Gonogo has a feature to LOCK the application against users.&#x20;

The locking of application can work in two ways

### AUTO LOCK

![](<../../.gitbook/assets/image (204).png>)

#### Applying AUTO LOCK

* If the application as no current users marked in front of it then the first user picking the application will be marked as current user. Check the red box
* If the application already has current user marked, then any other user is picking the case, that case will become read-only (non-editable).&#x20;
* As this locking works in auto-mode it is called as autolock

#### Release of AUTO LOCK

Release of lock will happen once the user will release the case. This may happen in two ways

* User logouts the application
* User goes to dashboard and picks other case

### MANUAL LOCK

User can also lock the case against his ID so that no other can update the case. This can be done by clicking the "Lock Case" button

![](<../../.gitbook/assets/image (203).png>)

Once user has completed the work, user can unlock the case by click the same button "Unlock Case" in the same menu. User can manually lock multiple cases against his ID

{% hint style="info" %}
Manual LOCK will not get removed by logging out of picking any other case.&#x20;
{% endhint %}

### How to check current user inside the case

Current user is shown on the top bar

![current user is shown on the top bar](<../../.gitbook/assets/image (205).png>)
