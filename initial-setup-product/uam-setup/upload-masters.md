# Upload UAM Masters

Below UAM masters are mandatory

| Master name             | UAM name             | Importance                                                                                                     | Sample                                                                                                          |
| ----------------------- | -------------------- | -------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| Branch master           | Branch Pool Master   | contains all the branch details like id, name, address, branch manager, location etc.                          | [link](https://docs.google.com/spreadsheets/d/1heJ5e-fx\_lzZ5B823LaxNt5S3KjiCmL8\_DbBem\_fBEQ/edit?usp=sharing) |
| Dealer / Agency master  | Dealer Branch Master | contains details of all the 3rd party agencies like id, name, [type](upload-masters.md#type-of-agencies)       | [link](https://docs.google.com/spreadsheets/d/1OnicMqwFIJRcxnCxTTQk2vrh4Pm7pzwxJRlt\_hlbXq0/edit?usp=sharing)   |
| Branch Hierarchy master | Hierarchy Master     | contains geographical hierarchy of the branches in 4 levels (branch -> Location -> Region -> Zone -> Country   | [link](https://drive.google.com/file/d/11ClWXFjqaci5YhEsGpYvjrFYUadCpMMg/view?usp=sharing)                      |

{% hint style="info" %}
Description of each column in the master is present in the master. All the columns marked in yellow and labelled as mandatory should contain some values. &#x20;
{% endhint %}

## Process to Upload masters

* Click on **Uploads** in Left navigation panel
* Select the master which you want to upload
* Click **Browse** and upload the file from your laptop
* Click submit

![](<../../.gitbook/assets/image (36).png>)

### Type of Agencies

| Type               | Desc                                                                                      | Screen Name                                      |
| ------------------ | ----------------------------------------------------------------------------------------- | ------------------------------------------------ |
| FIELD\_VERIFIER    | Applicable to agencies who perform FI , CPV, Address Verification                         | Field  Inspection                                |
| PROPERTY\_VERIFIER | Applicable to agencies who perform Property Valuation check (also called technical check) | PropertyValuation                                |
| LEGAL\_VERIFIER    | Applicable to agencies who perform Legal check                                            | Legal Verification                               |
| RCU\_VERIFIER      | Applicable to RCU, RIC, Fraud, document verification agencies                             | RCU Check                                        |
| TVR\_VERIFIER      | Applicable to Tele calling users and agencies                                             | TVR                                              |
| PD\_VERIFIER       | Applicable if PD is outsourced and is parellel                                            | Personal Discussion - Credit (one on left panel) |

