---
description: Workflow helps you to organize the API calls and stages in a sequence
---

# Workflow

Workflow helps you to determine what is going to be the sequence of the stage / status changes as per the events configured in the system.&#x20;

Example: SALES → CPA → CREDIT → CREDIT\_CHECKER → OPS → DISBURSED

The workflow consists of multiple sections of which description is mentioned below.&#x20;

## **Create Workflow**

![](<../../../.gitbook/assets/image (172).png>)

* User needs to enter the workflow name.&#x20;
* Users can enter _any name_ for your understanding. The workflow type will be MAIN right now.&#x20;
* Users can add nodes in the workflow. Each node determines what will happen at any specific event.&#x20;

## **Node List**

All the existing nodes are shown in a sequencial order.&#x20;

* If Node List is empty then click on Add Node button ![](<../../../.gitbook/assets/Screenshot from 2020-12-21 12-14-03.png>) &#x20;
* If new Node is to be added in the existing list then click on **"+"** button ![](<../../../.gitbook/assets/Screenshot from 2020-12-21 12-14-14.png>)&#x20;
* Users can add any node in between the two existing nodes or even add nodes at the end

![](<../../../.gitbook/assets/image (173).png>)

## **Inside a Node**

{% hint style="info" %}
Remember: One Stage = One Node
{% endhint %}

### **Section1: Node Basic Details**

![](<../../../.gitbook/assets/image (174).png>)

| **Field**        | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Node ID          | Auto incremented ID by the system                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Node Name        | Name for user understanding. This name will be visible in the [Node List](./#node-list)                                                                                                                                                                                                                                                                                                                                                                                                       |
| Node Type        | <p>Select the appropriate node type from the list</p><ul><li>STAGE: If the node is created to change the Stage / Status of the case on <strong>SUBMIT</strong> event</li><li>DECISION: if the node is created to change the Stage / Status of the case on <strong>Approve / Decline / Hold</strong> Events</li><li>SCREEN: If the node is created to change the Stage / Status of the case on the event of screen level API call.  </li><li>RECOMMEND: [Depricated]. No longer used</li></ul> |
| Node Events      | <p>Select the Events from the dropdown</p><p></p><ul><li>SUBMIT: To be selected when Type = STAGE</li><li>SAVE: To be selected when Type = SCREEN</li><li>Approved / Decline / OnHold: To be selected when Type = DECISION</li><li>offer-Accept / offer-Decline: To be selected when Type = DECISION</li></ul>                                                                                                                                                                                |
| Value            | Select the value of the Event from the dropdown. This is mandatory if the Node Type = SCREEN. This value will contain the respective screen API call. Example: For Sourcing screen API is `/registration`                                                                                                                                                                                                                                                                                     |
| Current Stages   | <p>Select the appropriate stages for the node to be executed. You can select multiple stages.This is <strong>important</strong> and has to selected correctly. <br></p><p>Example - If the Node Current Stage value  = Sales, then the node will only be executed for the case who will be having the same stage. <br><br>Note: Node will <strong>not</strong> get executed even if the other values match.  </p>                                                                             |
| Current Statuses | Select the appropriate stages for the node to be executed. You can select multiple statuses (Optional)                                                                                                                                                                                                                                                                                                                                                                                        |
| Next Stage       | <p>Select the next stage to be changed if the node is selected. (Mandatory)</p><p></p><p>Note: If you dont want stage to be change, you can select the same value as that of Current Stage</p>                                                                                                                                                                                                                                                                                                |
| Next Status      | <p>Select the next status to be changed if the node is selected. (Optional)</p><p></p><p>Note: this is optional</p>                                                                                                                                                                                                                                                                                                                                                                           |

#### Selection criteria of the node

Node will only be selected by the code and executed if the below conditions are matching&#x20;

| Node Type | Selection Criteria                                                                                             |
| --------- | -------------------------------------------------------------------------------------------------------------- |
| SCREEN    | <ul><li>Node Value (API name)</li><li>Current Stage</li><li>Current Status</li><li>Node Event = SAVE</li></ul> |
| STAGE     | <ul><li>Current Stage</li><li>Current Status</li><li>Node Event = SUBMIT</li></ul>                             |
| DECISION  | <ul><li>Current Stage</li><li>Current Status</li><li>Node Event = Approve OR Decline OR OnHold</li></ul>       |

If all the value entered then only Node will be selected.&#x20;

### **Section2: Node Condition**

{% hint style="info" %}
This section is difficult to understand and it has dependency on the code part. Try reading it multiple times.&#x20;
{% endhint %}

![](<../../../.gitbook/assets/Screenshot from 2020-12-21 12-33-24.png>)

This section will help to make the execution of the node **conditional.**

* Click on Add Node condition to add ![](<../../../.gitbook/assets/Screenshot from 2020-12-21 12-35-43.png>)&#x20;
* Multiple conditions can be added to a node.

![](<../../../.gitbook/assets/image (175).png>)

#### Flow Understanding&#x20;

* Multiple Node Conditions always works in **OR**. The code will check if the first condition is fulfilled, else it will go to the next Node condition
* Inside a Condition, multiple "Sub Condtions" can be added. These Sub conditions always work in **AND**

{% hint style="warning" %}
Understand this **AND / OR** logic very clearly
{% endhint %}

![Sample Flow for understanding](<../../../.gitbook/assets/Screenshot from 2020-12-21 13-36-48.png>)

**Description of Input Fields**

| Field                                | Desc                                                                                                                                                                                                                                                                                                                                                                                     |
| ------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Type (In Sub Condition)              | Select TYPE\_CONDITION always                                                                                                                                                                                                                                                                                                                                                            |
| App Condition Key (In Sub Condition) | <p>Select the value on which condition needs to applied</p><p>List and desciption of all the conditions is <a href="https://docs.google.com/document/d/1tfQIiwmrlKwzi4OJ3JDHwVHGNcm6Iy0VYiQvMQl7xZc/edit?usp=sharing">here</a></p>                                                                                                                                                       |
| Operator (In Sub Condition)          | <p>Select the correct Operation</p><ul><li>equals : Will check for Equality</li><li>nEquals : Will check for Non-Equality</li><li>in : Will check if the  value is present in the list of values</li></ul>                                                                                                                                                                               |
| Condtion Value (In Sub Condition)    | <p> Values for the Operator can be entered. Multiple values can be entered using comma Seperation</p><p></p><p>Ex - Sales,Credit. <em><strong>Do not enter spaces</strong></em></p>                                                                                                                                                                                                      |
| Impact Attribute                     | <p>Select the Field on which the change has to be updated. Ex - If you want Stage to be changed then select Stage from the dropdown</p><ul><li>STAGE : Select if you want to only change stage</li><li>STAGE||STATUS : Select if you want to change stage and status both. In this case you need to enter both the values in true and false value fields using pipe seperation</li></ul> |
| true Value                           | <p>Enter the Value in case the Node Condition becomes true. Multiple values can be entered using Pipe Seperation</p><p>Ex - Sales||Credit. <em><strong>Do not enter spaces</strong></em></p>                                                                                                                                                                                             |
| false Value                          | <p>Enter the Value in case the Node Condition is not true. Multiple values can be entered using Pipe Seperation<br>Ex - Sales||Credit. <em><strong>Do not enter spaces</strong></em></p><p></p><p>If False value is not required then enter "<strong>NA"</strong>. This will not change anything even if the conditon is false </p>                                                      |

#### List of Available Node Conditions: [here](https://docs.google.com/document/d/1tfQIiwmrlKwzi4OJ3JDHwVHGNcm6Iy0VYiQvMQl7xZc/edit?usp=sharing)

{% hint style="info" %}
All values are mandatory in Node Condition
{% endhint %}

### Section3: Interface Condition

![](<../../../.gitbook/assets/image (176).png>)

This section is used to check if the necessary conditions are fullfilled for executing [interface Configuration](./#section-4-interface-configuration). If condition is not fulfulled, then execution of the interface configurations in not done.&#x20;

The structure is same as [Node Condition](./#section-2-node-condition)

<mark style="background-color:orange;">List of Conditions</mark> is available [here](https://docs.google.com/document/d/1tfQIiwmrlKwzi4OJ3JDHwVHGNcm6Iy0VYiQvMQl7xZc/edit?usp=sharing)

### Section4: Interface Configuration

This is used to link APIs and Executors to the parent API.&#x20;

Ex - If LMS API is to be called after the Disburse Event, then the link can be mentioned here.&#x20;

{% hint style="info" %}
Details document on Interface configurations is [`here`](https://docs.google.com/document/d/1VyCEJhMjgardJ6k3u5RWIIAzakesF261wNy87S3vJhk/edit?usp=sharing)``
{% endhint %}

![](<../../../.gitbook/assets/image (266).png>)

#### Types of Interfaces

| Interfaces              | API calls are Synchronous and will be called as trigger to the parent API |
| ----------------------- | ------------------------------------------------------------------------- |
| Async APIs or Executors | These are a-synchronous and will work in background                       |

#### Input Fields Details

<mark style="background-color:orange;">List of Executors</mark> is [here](https://docs.google.com/document/d/1VyCEJhMjgardJ6k3u5RWIIAzakesF261wNy87S3vJhk/edit?usp=sharing)&#x20;

| Interfaces                          | List of APIs (multi-select). List of all Interfaces is [here](https://docs.google.com/document/d/1VyCEJhMjgardJ6k3u5RWIIAzakesF261wNy87S3vJhk/edit?usp=sharing)                                                                                                                                           |
| ----------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Wait for the A-Sync APIs response ? | <p>If Yes, then the Async APIs will make the parent API wait till the response is recieved. That means, on the UI, user has to wait for a longer time. </p><p></p><p><strong>Recommended</strong>: To keep it <strong>No</strong></p>                                                                     |
| Component Name                      | Select the Executor name                                                                                                                                                                                                                                                                                  |
| Component ID                        | Select the Executor name                                                                                                                                                                                                                                                                                  |
| Co-applicant                        | \[Depricated]. Enter any value                                                                                                                                                                                                                                                                            |
| Active                              | Select _true_                                                                                                                                                                                                                                                                                             |
| Policy Name                         | <p>Enter Extra details which are required from some of the executor</p><ul><li>Dedupe: Enter Dedupe Vendor name</li><li>SMS: Enter Template Name</li><li>Sobre: Enter <a href="../../module-level/eligibility-sobre-mapper.md">Sobre Mapper</a> Policy Name </li><li>Email: Enter Template Name</li></ul> |
| Execution Base                      | Only application to SMS and Email executors                                                                                                                                                                                                                                                               |

### Section5: Validation Condition

This section is used to check if the necessary conditions are fullfilled. If not, then you can throw customer validation message (highlighted in red) on the screen using this section

The structure is same as [Node Condition](./#section-2-node-condition)

List of Conditions is available [here](https://docs.google.com/document/d/1tfQIiwmrlKwzi4OJ3JDHwVHGNcm6Iy0VYiQvMQl7xZc/edit?usp=sharing)

![](<../../../.gitbook/assets/image (169).png>)

## Section6: Sub Workflow

All the API calls happening in one stage can be added here . The structure is same as that of a node.&#x20;

If you remember, we defined the node as one stage. So further if the stage has to be divided, then sub workflow can be used.&#x20;

Example: For stage DE, if you want to further add workflow for each API then you can used Sub Workflow.

{% hint style="info" %}
This Section is optional
{% endhint %}

![](https://lh3.googleusercontent.com/FdpDdE6Vq8EZ1M9sD0vTMBNV6kaRartQBeDf4X1IbiAYr1fkPt5eOLEKfK4MQV0M1tD0FozK7eicERE0lPuKIOXYCGMxiq8xLJG3YTj8NkAWZG0\_P1N4FUf1wT0d0H8z2lYbKhtP)
