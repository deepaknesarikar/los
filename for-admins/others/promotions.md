---
description: Copy Configs from lower to higher environments
---

# Promotions

Promotions will help you to move configs from one environment to other. Example: You can copy configs from SIT to UAT

### Process

#### Step1

From the lower environment click on the send icon. This icon will only be showed after you hover on the config box

![](<../../.gitbook/assets/Screenshot from 2021-05-24 14-36-30.png>)

#### Step2

You will get a pop-up with all the target environment available for promotion

![](<../../.gitbook/assets/image (195).png>)

Select the correct institute for promotions. And click **Save**

#### **Step3**

Go to Target environment in the promotions tab. You will see all the configs which are promoted in the table

![](<../../.gitbook/assets/image (196).png>)

You can perform below actions on the promoted configs

1. **View**: This will show you all the data present in the config. Note this will be in json format
2. **Approve**: This will approve the config and it will get stored and accordingly gonogo will change.&#x20;
3. **Delete**: If you have wrongly promoted the configs, then you can delete the configs

### Additional Filters

* Untick Institution Id if you want to approve "Lentra" level configs
* Tick product if you want selectively view configs which for specific products only

{% hint style="danger" %}
If wrong configs are approved , then if may creates functional bugs on the target gonogo environment
{% endhint %}

{% hint style="info" %}
Master name for admin promotion url at lentra level masters = environment\_master
{% endhint %}

## Restore (Backup) previous Versions

All the previous versions after the promotion can be seen in the Backup Promotions tab

![](<../../.gitbook/assets/image (256).png>)

The process works as below

1. Lets say their are configs A already available on UAT and config B on SIT
2. You promote Config B from SIT to UAT
3. Then  on UAT you will see config B and in backup promotions of UAT you will Config A

#### Actions

* View Backup Configs: You can view the json file of the config here
* Restore : This enable you to restore the previous version



