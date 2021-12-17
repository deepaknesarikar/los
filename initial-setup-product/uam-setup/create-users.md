# Create Users

## Process to create Users

1. Click on Users in the left panel
2. Click on " + " button
3. Enter the form details as below

* **First and Last name**: Will be used to display after login
* **Mobile** No: 10 digit is required
* **Email** : Will be used to send password on the email
* **Role**: Select the appropriate role.&#x20;

{% hint style="info" %}
It can also support _multiple roles_ for single user. To enable this please contact UAM team&#x20;
{% endhint %}

* **Dealers**: Dealers are only required for two types of users. For details [refer](../../for-users/others/agency-movement.md)
  * User who will trigger case to agency
  * Agency users to recieve the case&#x20;
* **Branches**: Assign single / multiple branches to the users. &#x20;
* **Products**: Select single / multiple products for the user to access case
* **EmployeeID:** Enter employee ID.&#x20;
* **User ID / Login ID**:  Enter user ID which will be used by users to login to GNG

![](<../../.gitbook/assets/image (33).png>)

## Use of Masters

#### Dealer Master:&#x20;

Dealer master contains the Agencies names. Important facts to remember while create dealer master are

* The agency has to be product wise. Hence, if same agency works for two products, the agency has to present twice with the different products
* Dealer ID , Dealer Name and Type are most important. Dealer should have approprite type.&#x20;
* In case dealer does multiple types of verifications then it has to be repeated per type once.&#x20;

**Allocation of Dealers**

1. For Triggering users:  Map the agencies to the user who eligible to trigger to them. You can map multiple agencies here
2. For Agency employees: Map the agency where the user is working. Here you need to map only one agency.&#x20;

### Branch Master

This master will be used to assign branches to the respective users. You can map multiple branches.&#x20;

{% hint style="info" %}
In case of multiple branches are assigned then a dropdown will come for selecting the branch for punching the case
{% endhint %}

### &#x20;Hierarchy Master

Hierarchy will help user to map to multiple higher levels. This master is non-mandatory &#x20;

Ex - if a user is Zonal Head, then instead of assigning him all the branches in the zone, you can directly assign him at zone level.

**Process**&#x20;

* Select the hierarchy type. It will show product for which hierarchy master is uploaded
* Select one of the level.&#x20;

![](<../../.gitbook/assets/image (34).png>)

* Select Hierarchy Value. You can select multiple here.&#x20;

![](<../../.gitbook/assets/image (35).png>)

{% hint style="warning" %}
This mapping has to be correct in order to show the cases as per the respective branches.&#x20;
{% endhint %}
