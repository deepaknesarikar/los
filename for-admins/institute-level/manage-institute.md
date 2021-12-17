---
description: Configure Institute parameters like logo color scheme etc.
---

# Manage Institute

Manage Institute will help you to configure the institute parameters which are mentioned below

![](<../../.gitbook/assets/image (261).png>)

#### Important Parameters

| Parameter      | Desc                                                                                                                                                                                                                     | Possible Value  |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------- |
| Institute Name | Used in all the places where institute name is required. Ex - in NACH form generate                                                                                                                                      | ABC Finance Ltd |
| Institute ID   | Auto capture and non-editable                                                                                                                                                                                            | 4000            |
| **Logo URL**   | <p>Enter the url of the clients Logo. This will be used to show on screen and in NACH form</p><p></p><p>Preview of the logo is also shown.<em>In case the preview shows error, that means the logo url is wrong</em></p> |                 |

#### Other Parameters

| Currency Short code                     | Not in use                                                                                                                                                                                                                                                                                                                                                                                                                                                        | USD / INR                |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ |
| Currency Symbol                         | Not in use                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Rs. \| $ \| **₹**        |
| Decimal Places                          | Not in use                                                                                                                                                                                                                                                                                                                                                                                                                                                        | 1/2                      |
| Comma Seperators                        | Not in use                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Indian / Thousand        |
| Date format                             | Not in use                                                                                                                                                                                                                                                                                                                                                                                                                                                        | yyyy/mm/dd \| dd/mm/yyyy |
| Primary Color                           | Currently only used for self serve                                                                                                                                                                                                                                                                                                                                                                                                                                | Select from dropdown     |
| Secondary Color                         | Currently only used for self serve                                                                                                                                                                                                                                                                                                                                                                                                                                | Select from dropdown     |
| File upload Size                        | Used for Assited. Default size will be 10 MB. Enter value other than 10 will change the upload limit                                                                                                                                                                                                                                                                                                                                                              | 10 / 20 / 30             |
| **Important : Sobre Verification Flag** | <p>If this is marked as <em>True</em>, then the Verify buttons will only be shown on the UI if sobre is giving the flag as true. If the value is anything other than 'True' then the buttons will be hidden even though they may be true in Configure Forms</p><p></p><p><mark style="background-color:orange;">Details Document</mark> <a href="https://docs.google.com/document/d/1n2x8Fm9RhNoq0s3VO2DqMygjkemkBIEkFzTlKY1LUBA/edit?usp=sharing">Link: </a></p> |                          |

#### Self Serve Parmeters

![](<../../.gitbook/assets/image (252).png>)

| Parameter       | Desc                                                                                                                                                                                                                                                       | Example Value       |
| --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------- |
| Header Text     | Shown on the landing page of selfserve                                                                                                                                                                                                                     | Welcome to ABC      |
| Help Text       | Shown on the landing page of selfserve                                                                                                                                                                                                                     | Get loans in 5 mins |
| OTP digits      | To quatify OTP digits as per the vendor                                                                                                                                                                                                                    | 4 / 5 / 6           |
| Default Product | <ul><li>This product will be used for sending login OTP to the customer. </li><li>Because product selection happens after successfull OTP verification, we require some default product.</li><li>Ensure this product is one of the real products</li></ul> |                     |

{% hint style="info" %}
To capture the Logo URL.&#x20;

1. Go the clients Website
2. Right click on the Image and select "Copy Image Address"
3. Paste the copied URL in the Logo URL field

Ensure the url is _**https**_ and has extentions from the this list _**(png / svg / jpg / jpeg)**_
{% endhint %}

