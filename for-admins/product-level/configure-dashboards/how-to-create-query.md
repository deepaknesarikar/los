---
description: Process for creating Dashboard Logic
---

# How to Create Query

## **Step 1:**&#x20;

Click on adding Rule or Ruleset as per the requirement. Already the first rule set will be added on the screen.&#x20;

![](https://lh6.googleusercontent.com/Kvm1p-Pf5drwnUdpL22tlDNLteDKqUpUm55MFRDoUw6QHGXKcbuJvYdQoWG6w9X4jWL2xlgQKv1yn3T68MsFjphpb7B5GL77a\_pbAdVhS1nTqlANRq6P74LahvLOUVYJKzauTing)

`Rule = Just one equation`

`Ruleset = Group of equations joined by AND or OR`&#x20;

{% hint style="info" %}
Remember: Ruleset can contain rules or other Ruleset
{% endhint %}

## **Step 2:**

Select the left hand side of the equation which is the field name. Select the appropriate [field](./#list-of-fields) from the dropdown.&#x20;

![](https://lh3.googleusercontent.com/YcIt3T7vNzebFSYaZMlUqDGP5As0blvRwM1uilRiscloXuE6NIU8IfhAk8obv3BQwttst8LLInPwzMSqkvqPaFTZ8FeEoS6cBip-NZ1ty9NpCh-LZGb07nH-a7UnvsIrIjfUVu-W)

## **Step 3:**&#x20;

Select the correct [Operator](./#operator-types) for the field**.**&#x20;

{% hint style="info" %}
Note: If you are going to get multiple values from the login response, then you need to select IN as operator. Use IN for Branchname / zone / region / branchid &#x20;
{% endhint %}

![](https://lh3.googleusercontent.com/7heyBIgc8BlfiHpTgaeXeRAkah1dbKqJaP7YWSNOyiv7H74m\_RoyIB86cuqdLB67lcZ246gdeRVXgJv5bsJUM9OuyAqMoIMT4fkF9OOJNzU39Jj03714B0ZVuMXkq07mqysl\_Lll)

## **Step 4:**&#x20;

Select the Right hand side of the equation **** based on the [type](./#list-of-fields) of the field\


**For UI request Type**

![](https://lh6.googleusercontent.com/GTC1DOqegUGD8Ez179Iph4Tf60dag\_9\_U3RSlCD2zB9rYEqGmeXvKi8neSmLrwnWpnw98mH8xvLjki09c74wHYiQ20DTbqdHoeSD\_T39n9ANa6mpCGU9\_fGgoJJf5g70R4cvV0uC)

**For Dropdown Values**

![](https://lh4.googleusercontent.com/SMMZ0HZ5j3v4JSFFgA-gsz2a3R-pasa6WJyXdr2I67Mc6WrooJKDHTNL\_-9pBlxTH\_K3DUw8kySa6bXn4OuSUnS3cSWcAa3y\_CfDWYc77useaS\_cdXfFYSulsezj6o2abR08afi9)

**For User Input**

![](https://lh3.googleusercontent.com/wPytnJPdXmTtbGTO9ikUKvL5KMKZZzId3m5r9VL6X6QG91WugHRK4H-rfb1BrgdVtWBiR\_YBbobywJDlXKwArqgDjSDY3eY8Qei5jJrl-JBg9nd5BEAH240Az9aRe4SxRw9lKiJs)

## **Validations**

* Each Role can have one Dashboard per type.Ex -  One for MY and one for ALL
* Operator IN will work if you are matching one value with multiple values and vice versa. For one to one matching use “IS”
* If the dashboard does not load, then please contact the dev team.&#x20;
