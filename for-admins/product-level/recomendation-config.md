---
description: Add Role wise Sendback / Recommendation Configs
---

# Recomendation Config

&#x20;\
**Business case**: If Credit finds something incomplete in the case, then credit can send back to the the Sales stage in two ways

* Role level: User will select the role which is associated with Sales and then send it that role. The stage of the case will be changed and case will accordingly will be visible to that role&#x20;
* User level: user will get a dropdown of all the users in that role, so that the case gets allocated to a single role. The case will only be editable to that specific user. &#x20;

## Process to Add Configs

### **Step 1:**&#x20;

Select the existing or click on plus button to create new

![](https://lh6.googleusercontent.com/KOEDfQnwWL5ILN1xegmgMaWkSQlMXoN6MbWtLwzguNkVvE-9POL0KmqNd3pHH2tgsku\_90W6ey7IXg3Z6xw1zb5zasUqo7jWhsV\_BZ193Xs6M\_OolK9T\_H03dRjuGLOPoGcWUl\_b)

### **Step 2:**&#x20;

Select the Role which you want to save the recommendation config in “Recommendation From Role”&#x20;

### **Step 3:**

Select the “Recommendation From Stage” and “Recommendation From Status” for which you want to allow that role to recommend the case

{% hint style="info" %}
Note: “Recommendation From Status” is optional. Select NA. \`\`
{% endhint %}

![](https://lh4.googleusercontent.com/fc51\_rE5Wp2THEPqQF0Pr9IjsXVC8B5lIMWB3mJxVNXNkPgbbNCIOToqJN8PdSgLM5KZLFpNMOGDEujdFfwv\_d3bL1bwrW\_7U2vULeQv3ww-MXcgiZrFa\_5OIGWFy0oap3lVsCNw)

### **Step 4:** ****

![](https://lh3.googleusercontent.com/y1JfPe9ADs6QgZ3GShksITjD7KVS9eJbIFaiRO-dgH8W1\_paakBUa6SsXdARe8NaMWhoxRz2\_bwAF5l7z2K6tz1ZXQ75j9blovdPQ9RY2K-LpCoE6t8qI7Qy6azGtVVrZ2n0FkS4)

1. Add the Roles to which the From Role can send the cases. The roles dropdown will come from the UAM
2. Select the stage which you want to be changed to. Once the case is recommended, then the application stage will change as per the selection
3. Select the status which you want to be changed to. Once the case is recommended, then the application status will change as per the selection
4. Select the type of recommendation should be allowed for that respective rule. The options are as below
   1. **USER\_WISE:** For the selected role, the case will be sent back using the user selection
   2. **ROLES\_WISE**: For the selected role, the case will be send back using the role as dropdown
   3. **SALES**: This can be selected only if the USER\_WISE is selected. This has to be ticked if cases has to be only shown to the user who has punched the cases. ****&#x20;

![](https://lh3.googleusercontent.com/6o1P2T0qLmtxCtNt2Co68onD4ExzkpKyGaTCkInKmbEyw4G59c0pRQotPtOwSymAtkJwp6Ho34wgdsQmC2fRB65r7CGC4McS4wzGLGF1yha\_shGhScKD2m4uh98RNtaAfmQTcPEb)
