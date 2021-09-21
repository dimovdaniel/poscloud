# FAQ - Business

## Can I use Lion POS in QR Menu Maker, WhatsApp, or FoodTiger?

Lion POS comes with the following modules. 

1. Floor Plan
2. POS \( exclusive so LionPOS \)
3. Staff
4. Expenses

They are located in **modules** folder

You can zip these modules one by one and upload them in QR Menu Maker. So you will get the POS functionality in QR Menu Maker. Unfortunately, WhatsApp and FoodTiger are not compatible.

{% hint style="info" %}
Make sure you use version 2.7.3+ of QR Menu Maker for full compatibility.
{% endhint %}

## Can I use Lion POS landing page in QR Menu Maker, WhatsApp? 

From v2.7.3+ yes, you can. And here is how. 

Copy and paste from Lion POS to QR Menu maker or WhatsApp project

* public/soft
* resources/views/poslanding
* resources/lang/en/poslanding.php

After that, open the .env of QR Menu Maker or WhatsApp and add this two records

```text
SHOW_LANDING_MANAGMENT=true
LANDING_TO_USE=pos
```









 



