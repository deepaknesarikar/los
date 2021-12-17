---
description: Add more configurations to your roles
---

# Advance Role Configs

The advance role configs will help you to maintain more parameters associated with the institute roles.&#x20;

All the Active (enabled) roles can be used to add them the advance configs. The configs are as below

| Config            | Desc                                                                                                                               |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Select Role       | Select the Role for which you have to add config                                                                                   |
| Department        | Write the department of the role                                                                                                   |
| Reports to        | Select the Role which is supervisor. This is important for role wise hierarchy management                                          |
| Is 3rd Party Role | Tick this if you want this role to work in the cases parellely with any other role.                                                |
| Approval  Limits  | <p>Approval Amount: Enter approval amount for this role </p><p>ROI: Enter ROI for this role</p><p>LTV: Enter LTV for this role</p> |

![](<../../.gitbook/assets/image (167).png>)

{% hint style="info" %}
Is 3rd Party Role should only be enabled for Roles which are generally agency and function parellelly with any other role.&#x20;

Example: If FI has to work along with Credit person, the FI role has to be marked as 3rd party Role
{% endhint %}

## Role Hierarchy

Once user entered the Reports to role in the advance role parameters, then user can come to this screen and then click on "Sync Hierarchy". &#x20;

![](<../../.gitbook/assets/image (217).png>)

This will create a hierarchy in the backend and who it on the top

* The person at the top-most level is kept as L1
* The lower the hierarchy, the levels will increase

This is currently use in

1. Case [assignment](../../for-users/others/dashboard.md#dashboard-queue) Dashboard: The supervisor role can allocate cases to the users of his reporting roles. Ex: in the above screenshot `CYOR_INSTITUTION_ADMIN`can assign cases to `UM_SUPER_ADMIN`
2. Deviation Approval (in development)
