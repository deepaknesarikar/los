---
description: Create Reports and CAM
---

# Templates

Templates will help you to create screen reports / Views and PDFs by pre-populating the application data in it.&#x20;

### Steps to create new template

Click on "+" button

![](<../../.gitbook/assets/image (250).png>)

1. Enter the Template name.&#x20;
2. Select the Document Type
   1. Document
   2. Custom\_Document
   3. Email
   4. SMS
   5. SMS\_OTP
   6. CAM
   7. Email\_OTP
3. Library Type: This is only available for Document Type = Document or Custom Document. Select the library you want to use for data prepopulation
   1. Moustache: Logic less, can be used for simple templates
   2. Freemarker: powerful for if conditions and data transformation. Can be used for complex templates
4. Enter Template Display Name. This will be visible on the GoNoGo Screen
5. Select Product: Select the one / multiple product for which this is applicable
6. Select Role and Stage: Select the one / multiple role stage for which this is applicable
7. Enter Source code: Enter the HTML of the template which also contains the variables mapped
8. HTML editor: Non technical persons can use this for viewing the HTML or converting google doc to HTML

{% hint style="info" %}
Default library used in _Moustache_ for all the documents types. &#x20;
{% endhint %}

### Steps to create template

1. Create the template in google doc.&#x20;
2. Copy the content in the template in paste in this link: [https://onlinehtmleditor.dev/](https://onlinehtmleditor.dev)
3. Map the fields using the json key. For learning how to map the db keys, connect with developers
4. Click on  ![](<../../.gitbook/assets/image (184).png>) and copy the html in the templates.&#x20;

![](<../../.gitbook/assets/image (185).png>)

{% hint style="warning" %}
Ensure the variables are  entered correctly. Then only the fields will be pre-populated in the template
{% endhint %}

## Templates capabilities

* Moustache: [https://mustache.github.io/mustache.5.html](https://mustache.github.io/mustache.5.html)
* Freemarker:[https://freemarker.apache.org/docs/dgui\_quickstart.html](https://freemarker.apache.org/docs/dgui\_quickstart.html)

### Standard GoNoGo JSON for type = Documents

<mark style="background-color:orange;"></mark>[<mark style="background-color:orange;">Document Link</mark>](https://drive.google.com/file/d/1cVKHv7tjsypFNiBbh3vC6fjvyr0uLcKl/view?usp=sharing)<mark style="background-color:orange;"></mark>

#### To Know how about Generation templates in GoNoGo visit below link

{% content-ref url="../../for-users/others/templates.md" %}
[templates.md](../../for-users/others/templates.md)
{% endcontent-ref %}
