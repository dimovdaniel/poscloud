# Changelog

## 2.5.0 - 2021-06-19

### Video
{% embed url="https://youtu.be/J_mBypwyBl4" caption="" %}

### New
* Logo for restaurants in the header area

### Improvements
* Better SEO
* Items import
* Limit number of orders in plan

### How to update
Just log in as admin, go to "Updates" and you should see new "New Update 2.5.0" button. Click on the button to update. Note that this is a bigger update. Please check the List of files to confirm it will not overwrite some of your changes if you have them.

**List of updated files**

[File list](https://gist.github.com/dimovdaniel/fb8786456f106660b85ccbe3e58744af)


## 2.4.x - Continues updates

* 2.4.3 - Subscription fixes, Landing fixes, Import fixes  [Files](https://i.imgur.com/nmxO4ik.png)
* 2.4.2 - Local Bank fixes, decimal orders prevent, better whatsapp message [Files](https://gist.github.com/dimovdaniel/cb945997092427699ee7a811e265e61e)
* 2.4.1 - Local Bank fixes, Saving Stripe Fixes, Working Hours Fixes - [Files](https://gist.github.com/dimovdaniel/c0791ee6280805b30e1acd8eafddbb93)

## 2.4.0 - 2021-04-16

### Video

{% embed url="https://youtu.be/fkZZHYLLems" caption="" %}

### New

* Payment modules as Plug And Play
* Each payment method can be set so money from orders goes to vendor
* Restaurant management reorganization
* New Printing module
* vendors can set their own time slots intervals, prepare time and timezone

### Fixes

* Tax calculation fixes
* Lot of small fixes

### How to update

Just log in as admin, go to "Updates" and you should see new "New Update 2.4.0" button. Click on the button to update. Note that this is a bigger update. Please check the List of files to confirm it will not overwrite some of your changes if you have them.

If you have lot of users / clients and you are using other payment method for orders than Stripe, I will recommend full project backup, database and files. Afterwords you will need to download the desired payment method, and set up the way you like it. Please look into the update video to see what has been changed in the payment methods. Restaurants will need to reset the api keys for Mollie or PayPal if they where accepting direct payments.

**List of updated files**

[File list](https://gist.github.com/dimovdaniel/71f85505b15f776f1cd2e2e5b173d2a7)

## 2.3.x Continues updates

* 2.3.2 - Support for the impressum app. [Files](https://gist.github.com/dimovdaniel/45b4b2476896e2920550ef58c33bacab)
* 2.3.1 - Fix for restaurant orders \(array\_key\_exists\(\)\) - File changed: app/Order.php

## 2.3.0 - 2021-03-17

### New

* Apps \( instal new modules via upload \)
* Free app - invoice pdf printer 
* Owner API - API endpoint for owner actions

### Fixes

* Fixes for Financial reports
* Fixes for testimonials and 
* Other small fixes

### How to update

Just log in as admin, go to "Updates" and you should see new "New Update 2.3.0" button. Click on the button to update. Note that this is a bigger update. Please check the List of files to confirm it will not overwrite some of your changes if you have them.

**List of updated files**

[File list](https://gist.github.com/dimovdaniel/c1eaaacc8f36fa71ef44a4cbbdc26087)

## 2.1.x - 2.2.x - Continues updates

* 2.2.3 - Fix for handling restaurant-name like aliases -[Files](https://gist.github.com/dimovdaniel/6ebd98a48eba52906fb536dfd80d45e5)
* 2.2.2 - Fixes in calculating tax, Fixes in  financial report, add new item image missing - [Files](https://gist.github.com/dimovdaniel/a63e2dbabde132691d892430199a06f9)
* 2.2.1 - Custom Fields on orders, Social Links, Restaurant address improvements - [Files](https://gist.github.com/dimovdaniel/4e5e670a13bbcb52e1d1143f34752c44)
* 2.2.0 - Categories sorting, Fix for Stripe 3d secure or plan subscribe - [Files](https://gist.github.com/dimovdaniel/4e168f71933b3249a4e853e5f6995b21)
* 2.1.9 - Temporary update 
* 2.1.8 - Temporary update 
* 2.1.7 - Fix for restaurant save, Memory Limit info, Migrate in update - [Modified Files](https://gist.github.com/dimovdaniel/fcf3703ec281b69265869ad9b9953742)
* 2.1.6 - Fixes on variant show - [Modified Files](https://gist.github.com/dimovdaniel/90d555271a5db0c6f2cf7980e69befab)
* 2.1.5 - New way of updates, fixes in image upload in settings  - [Modified Files](https://gist.github.com/dimovdaniel/786c82b2776eda1d47a97a5ec9c970c4) -- \(YOU WILL GET ERROR 500 - but that is ok, since now we have new system for update \)
* 2.1.4 - WhatsApp Message is separate blade file - [Modified Files](https://gist.github.com/dimovdaniel/7a3fad29bf15241fe310fdecd8e0da68)
* 2.1.3 - Fixes in Stripe connect - [Modified Files](https://gist.github.com/dimovdaniel/644f827344deed01443309429f56a542)
* 2.1.2 - Missing Translations, Live Order fix, CSS fixes, Fix on deleting demo data -   [Modified files](https://gist.github.com/dimovdaniel/165ae8c25bbf1fce08cb5a2243127fef)

## 2.1.1  - 2021-02-10

### New

* WhatsApp Ordering

### Fixes

* Stripe 3D Secure
* HasDineIn Problem - when there is only dine in.

### Improvements

* Full list of currencies
* Better error 500 show
* Show/Hide Cookie Consent

### How to update

Just log in as admin, go to "Site Settings" and on right top you should new "New Update 2.1.1". Click on the button to update.

**List of updated files** [File list](https://gist.github.com/dimovdaniel/497727c35598c29d644b0a95c8d974de)

## 2.0.x  - Continues updates

* 2.0.7 - JS Notify Fixes, Don't show empty categories, Phone min.
* 2.0.6 - Translate plugin fix for PHP 8
* 2.0.5 - Fixes for orders - no action displayed
* 2.0.4 - Stripe Subscribe fixes
* 2.0.3 - Pusher fixes
* 2.0.2 - Site map generation and Stripe Connect fixes
* 2.0.1 - Fixes for Dine in option and small bug fixes

## 2.0.0 - 2021-01-15

This is a major update and is not available via 1 Click update. You will need to follow the guide for updating. **Note** that now, you need to change php version to 7.4 or 8.0.

{% embed url="https://youtu.be/FeN7\_c8k2kY" caption="" %}

### New

* Update to latest Laravel 8
* Redefined Ordering process
* Multilingual menus
* Option restaurants to change currency
* New install and 1 click update process
* Bug Fixes
* Easy way to add new payment methods

### Updating

To update from the previous release, follow the [standard update procedure](https://mobidonia.gitbook.io/mresto/changelog/updating-shared-hosting).

After that, log in as admin

## 1.9.7 - 2020-12-17

This is a combined update from 1.8.0 to 1.9.7

### Fixes

* Variant selection bug fix
* Call waiter pop-up select not showing fixed
* Plus button in the cart was not showing on mobile
* Updated menus privileges on the front end
* Delete user when an admin deletes restaurant
* Duplicate email send 
* Admin order accepting 
* Checkbox when placing an order to accept T&S
* Sound on pusher notification
* Category delete when there are no items
* Thank you page after successful payment
* Fixes for Paystack

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.9.X. Click on the button.

## 1.8.0 - 2020-12-05

### **New**

* Call Waiter button
* PayPal subscriptions
* PayPal payments
* PayStack subscriptions
* Mollie payments
* XML Sitemaps
* Close account and get all data in json
* Easy Share on web and QR

### **Improvements**

* Dark / Light logo
* Better ordering flow
* The correct menu is shown based on settings
* The phone number on takeaway order
* Password field was prepopulated
* Better settings screen
* EPS, PSD, JPEG, SKETCH files for the templates \( only from download from CodeCanyon \)

### **Fixes**

* Saving env adds new lines
* Language link doesn't work
* PayStack fixed
* Language selector on landing not showing selected language
* Deleting customer log entry results in an error
* 2 Emails where send to the restaurant on register

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.8.0. Click on the button.

## 1.7.9 - 2020-11-12

### Improvements

* Inline editing on the front page
* Customer can see orders they have made
* Remove Project branding from the restaurant menu page
* Options to disable Guest log
* Option to edit categories name in the menu
* Delete demo data button added
* Optin to completely delete restaurant
* Bugfix: When selecting variants, $ is US$
* Bugfix: Wildcard domain QR make
* Option to change required characters in a phone number

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.7.9. Click on the button.

## 1.7.8 - 2020-11-08

### Improvements

* Dine-in / Takeaway when making an order
* Option to not offer a free plan \( set FREE\_PLAN\_ID to 0 \)
* Images for a menu item, are no longer required
* Fixes on working with the variants
* Fixes on registering customer visit by the customer
* Deactivated restaurant, no longer accessible

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.7.8. Click on the button.

## 1.7.7 - 2020-11-01

This is a combined update from 1.7.3 till 1.7.7

### Improvements

* Change landing page images via settings

### Fixes

* Stripe system status check
* REcaptcha fix
* Plan removing fixes
* Fixes for managing options and variants

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.7.X. Click on the button.

## 1.7.3 - 2020-10-28

{% embed url="https://www.loom.com/share/15cc92bffca0416da783972f55bbce79" caption="" %}

This is a combined update from 1.5.8 till 1.7.3

### Improvements

* Tables and area management
* Local order \( Continuous orders and online card payments \)
* Orders \| Report and live orders
* Customer log
* Subscribe via stripe
* Manually assign restaurant to pricing plan

{% hint style="info" %}
This update introduces Stripe as default way for accepting subscriptions. To enable it, you need to register stripe account, and create product in it. When you create the pricing plans, you will need to enter Stripe pricing\_id for each plan.

New variables in .env

ENABLE\_STRIPE\_CONNECT=true  
ENABLE\_FINANCES\_OWNER=true  
ENABLE\_FINANCES\_ADMIN=true  
ENABLE\_STRIPE=true  
STRIPE\_KEY='pk\_test\_XXXXXXXXXXXXXX'  
STRIPE\_SECRET='sk\_test\_XXXXXXXXXXXXXXX',  
SUBSCRIPTION\_PROCESSOR=Stripe  
QRSAAS\_DISABLE\_ODERING=false
{% endhint %}

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.7.3. Click on the button.

## 1.5.8 - 2020-10-17

This is a combined update from 1.5.6 \| 1.5.7 and 1.5.8

### Improvements

* Google ReCaptcha added
* Better Favicon generation
* Better frontend language manager
* Limit plan fix
* Better URL route for restaurant edit
* Other small bug fixes

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.5.5". Click on the button.

{% hint style="success" %}
This update changes the config for the frontend languages

To modify the list of available language add new .env variable

FRONT\_LANGUAGES=EN,English,FR,French
{% endhint %}

{% hint style="success" %}
In this update we introduced the Google Recaptcha.  
We are using this [plugin](https://laravel-recaptcha-docs.biscolab.com/docs/intro) for Laravel. And we have implemented the invisible recaptcha.

To enable it on the registration form, you have to create your own API keys [here](https://www.google.com/recaptcha/admin).  
reCAPTCHA type:**v2 Invisible**

Then you need to enter thous keys in .env

in your .env file

RECAPTCHA\_SITE\_KEY=YOUR\_API\_SITE\_KEY RECAPTCHA\_SECRET\_KEY=YOUR\_API\_SECRET\_KEY
{% endhint %}

## 1.5.5 - 2020-09-30

### Improvements

* System setup status and better error handling
* Translation management
* Custom CSS and JS for frontend and backed set from the admin
* Landing page into separate files for easier update
* Gravatar image corrections

### How to update \( [Video](https://www.loom.com/share/bd05fb6bdceb46b3942bcf3b8e9f5e34) \)

Just log in as admin, and you should see "New Update 1.5.5". Click on the button.

{% hint style="warning" %}
This update will change your landing page. But your landing.blade.php file is not modified. Landing now uses home.blade.php and uses separate files to show content. We did this for easier future updates.

The content of the landing page is now in resources/views/qrsaas/partials

To show your old landing, just add .env variable  
QR\_LANDING=landing

To modify the list of available language add new .env variable

LANGUAGES={ "EN":"English","FR":"French"}
{% endhint %}

## 1.5.4 - 2020-09-29 \( test update \)

{% hint style="info" %}
This is the first incremental update that can be done via the 1Click Update button.  
If you receive an error like HOME ACTION NOT ALLOWED it is because you are logged in as admin, but the admin ID is not 1. Open config/laraupdater.php and at the bottom modify the variable allow\_users\_id to have the admin ID, or set to false to accept all admins.
{% endhint %}

### **Fixes**

* Paddle vendor id correct setup

## 1.5.3 - 2020-09-29

### Improvements

* One-Click update button 
* Favicon change setup from admin settings
* Removed more unnecessary fields in admin
* Fixes on the  menu on mobile phone
* Spelling mistakes corrected on landing
* Removed 40 00+ Unnecessary developer files
* Plan limit:  now prevent the user to add new items in the menu if the limit is reached

### How to update

Follow the standard update procedure

From this version on, when there is a new update, log in as admin, and you will see a blue card on left, indicating that there is an update you can apply.

{% hint style="warning" %}
This update brings updates on the landing page. if you have modified, you may want to back it before updating.
{% endhint %}

## 1.5.2 - 2020-09-24 \( [Video](https://youtu.be/gZ7WGhdOq5I) \)

### Fixes

* Better documentation 
* Option to add / change the print templates provided
* Option to translate the QR Maker page for restaurants
* Removed unnecessary fields and options for admin
* Categories Filter fixed
* Removed wizard option from the install screen
* Option to disable landing page DISABLE\_LANDING in .env

### How to update

Follow the standard update procedure

Or, here is the list of file modified, so you can change them one by one if you prefer.

{% embed url="https://1drv.ms/u/s!AqVDdjJrM4dRhoV2HokQUTkzOTlIqg" caption="" %}

## 1.5.1 - 2020-09-19

### Initial Version

