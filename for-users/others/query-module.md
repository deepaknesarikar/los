---
description: Raised and resolve queries
---

# Query Module

Queries are questions asked in the case without sending back the case. The raised queries are then shown as RAISED in the message button on top right.&#x20;

The queries are show at two places.&#x20;

1. On landing page: The message icon on landing page will show queries which are tagged to you and are in open (RAISED) stage
2. Inside the case: The message icon inside the case will show queries which are present in that case and are in open (RAISED) stage

The Stages for queries are as below

* RAISED (color = red)
* REPLIED (color = yellow)
* CLOSED (color = green)

## View Open queries

The shortcut to queries is the message pop-up. If there are no queries then the pop-up will be show "No queries pending"

![](<../../.gitbook/assets/image (242).png>)

Inside the application, the pop-up will be shown as below&#x20;

![](<../../.gitbook/assets/image (246).png>)

|   |   |
| - | - |
|   |   |

On the landing page, the pop-up will be shown as below. Note the difference in the title.&#x20;

![](<../../.gitbook/assets/image (247).png>)

## Raise new query

Roles who have access to raise new query button (Action name  = RAISED\_QUERY), can click on the raise query button and fill the information as shown below

![](<../../.gitbook/assets/image (243).png>)

{% hint style="info" %}
If Select User pop-up is blank, refer below steps to trouble shoot

* You need to perform [sync users](../../for-admins/institute-level/sync-users.md)
* There are no users for the selected branch
{% endhint %}

## Reply / Resolve queries

The list of queries will be visible if you click on "View all queries" button in the message pop-up. All the queries will be shown as below.&#x20;

![](<../../.gitbook/assets/image (244).png>)

User can perform below actions on the queries

![](<../../.gitbook/assets/image (245).png>)

| No | Action         | Desc                                                                                                                                                                                                                                 |
| -- | -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1  | Upload Image   | The user who has been tagged to the query can upload the image. Once image is uploaded the status will get changed to REPLIED                                                                                                        |
| 2  | Change Status  | <p>The status can be changed in below two ways</p><ul><li>Uploading image will change the status to REPLIED</li><li>Person who has raised the query can change the status from REPLIED to CLOSED by clicking on the button</li></ul> |
| 3  | Delete Query   | Only Person who has raised the query can delete the query                                                                                                                                                                            |
| 4  | Filter Queries | Queries can be filtered by using the filter button                                                                                                                                                                                   |
