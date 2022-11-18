# Changelog

## 3.4.x - Continues updates

* 3.4.1 Clone on item level - activated - change in resources/views/items/edit.blade.php and config/config.php


## 3.4.0 - 2022-11-12

### Video

{% embed url="https://youtu.be/mgJ-l95nAaI" %}

### New

* Admin menu reorganization

### Modules

* Clone module - clone single item
* Reintroduce TinyPNG module
  
### How to update

Just log in as admin, go to "Updates" and you should see new "New Update 3.4.0" button. Click on the button to update. Note that this is a bigger update. Please check the List of files to confirm it will not overwrite some of your changes if you have them. NOTE: For this update we strongly recommend to backup your database and files.

### List of updated files

[Updated files](https://paste.laravel.io/0bbe4bc1-ef8b-48c5-bb7f-c28272eb80b1)



## 3.3.x - Continues updates

* 3.3.1 Small improvements [Changes](https://share.cleanshot.com/EzvOZR) [Files](https://paste.laravel.io/6dfcd9f1-9daf-4682-87f0-ba4ace82e7a6)


## 3.3.0 - 2022-08-05

### Video

{% embed url="https://youtu.be/wgnqKEyjkPE" %}

### New

* Restaurant Search in Admin
* KDS compatible and KDS API
* On Address change, change location of vendor
* Community plugins
* API: Deactivate Account- APP
* Login as from vendor details
* Pusher event on order update

### Bugs

* Bug:When no orders, can't change filters
* Bug:Return only staff users in Staff List
* Bug:Options with special character or arabic
* Bug:Items import redirect to index page, and more robust import
* Bug:Saving Simple Delivery area without phone
* Bug:Stripe subscribe issues
* Bug:Landing page can't be disabled - error in saving .env
* Bug:Problematic image removed from pwa

### Modules

* [Kitchen Display System](https://www.loom.com/share/4a8460875c2c4d1aa0227ea94009de91)

### How to update

Just log in as admin, go to "Updates" and you should see new "New Update 3.3.0" button. Click on the button to update. Note that this is a bigger update. Please check the List of files to confirm it will not overwrite some of your changes if you have them. NOTE: For this update we strongly recommend to backup your database and files.

### List of updated files

[Updated files](https://paste.laravel.io/7dce0e61-8c18-4752-b906-3fbe7c5248c6)


## 3.2.x - Continues updates

* 3.2.2 Multiple fixes [INFO](https://share.cleanshot.com/rjhERB) [Files](https://gist.github.com/dimovdaniel/cdb1c3c252d1e06788a4f8716cb238ff)
* 3.2.1 Fix problem sending to Whatsapp [Files](https://paste.laravel.io/ce079a93-20c7-4ca1-8016-a3caf4477ada)



## 3.2.0 - 2022-03-20

### Video

{% embed url="https://youtu.be/tJTldQBxW4o" %}

### New

* Verify install and setup is ok
* Modules per pricing plan
* Better LoginAS
* Change  /restaurants - URL Route in admin

### Modules

* Drivers per vendor    
* Manager Module
* Tiny PNG - AWS S3 - Google Cloud
* MailChimp add users on new vendor
* Links in side menu of the vendor

### How to update

Just log in as admin, go to "Updates" and you should see new "New Update 3.2.0" button. Click on the button to update. Note that this is a bigger update. Please check the List of files to confirm it will not overwrite some of your changes if you have them. NOTE: For this update we strongly recommend to backup your database and files.

### List of updated files

[Updated files](https://paste.laravel.io/4062a600-893b-45ba-9334-c2bac45c2df2)

## 3.1.x - Continues updates

* 3.1.3 Register problem with recaptcha enabled fix [Files](https://paste.laravel.io/2c4cd9a8-4187-4193-921a-6fed48727193)
* 3.1.2 Register Vendor in admin and Vendor Finances fix in 3.1.0 [Files](https://paste.laravel.io/6a1da2e8-9ee8-4022-97af-c05010ea77b9)
* 3.1.1 Flags and  Finances fixes in 3.1.0 [Files](https://paste.laravel.io/a58c2b81-a9af-44e5-b092-56df0294d0b6)

## 3.1.0 - 2022-01-16


### Video

{% embed url="https://youtu.be/OxyhrtVz3ME" %}

### New

* Phone number input
* Improved apps page
* Staff can see live orders.
* Filter by order status and payment

### Fixes

* Owner can see the POS ( 1.4 )
* Stripe subscribe cancel button
* Other small bug fixes

### Modules

* Detrack module

### How to update

Just log in as admin, go to "Updates" and you should see new "New Update 3.1.0" button. Click on the button to update. Note that this is a bigger update. Please check the List of files to confirm it will not overwrite some of your changes if you have them. NOTE: For this update we strongly recommend to backup your database and files.

### List of updated files

[Updated files](https://paste.laravel.io/400952df-62f9-40b2-8380-0d6f8bb0b070)



## 3.0.x - Continues updates

* 3.0.6 - 3.0.3, 3.0.4, 3.0.5 + Language switch fix [Files](https://paste.laravel.io/0e424692-add2-4822-bc1f-52559fbbdbbf)
* 3.0.5 - POS fixes [Files](https://paste.laravel.io/06b893a6-ebee-41cd-b586-a30b8d46d0db)
* 3.0.4 - 3.0.3+ Small fixes. Error was made in the zipping of the update in 3.0.3 [Files](https://paste.laravel.io/8563ed64-4b02-4629-87ae-65a0480c145a)
* 3.0.3 - Remove apps, Vendor plan monthly order limit - file changed is config/config.php
* 3.0.2 - Fix bug on making order, Bug fix on logo save, No working hours[Files](https://paste.laravel.io/61619615-1d64-47f4-9e13-e7d18a3e89a2)
* 3.0.1 - Coupons Fix, Order change QTY fix, Coupons Deduction fix - [Files](https://paste.laravel.io/1cca9e36-bf76-4f62-860f-9b40db662861)

## 3.0.0 - 2021-11-08

### Video

{% embed url="https://youtu.be/tvwLPyzpqP4" caption="" %}

### New

* Online Payments
* New apps organization
* Modify Qty on each item in order
* Force users to paid plans
* Disable pickup/delivery.
* Compatible with new modules and easier to make design changes on menu

### Fixes

* Lot of small bug fixes

### Modules

* [Custom Domain](https://mobidonia.gumroad.com/l/COWDi)
* [Coupons](https://mobidonia.gumroad.com/l/djizl)
* [Prepare Time](https://mobidonia.gumroad.com/l/kyFdp)
* [Default tax](https://mobidonia.gumroad.com/l/defaulttax)
* [Language Pack](https://mobidonia.gumroad.com/l/languepack)


### How to update

Just log in as admin, go to "Updates" and you should see new "New Update 3.0.0" button. Click on the button to update. Note that this is a bigger update. Please check the List of files to confirm it will not overwrite some of your changes if you have them.
NOTE: For this update we strongly recommend to backup your database and files. 

### List of updated files
[Updated files](https://paste.laravel.io/a4bed46b-b8cc-49bd-be87-61ba88a29e41)

## 2.7.x - Continues updates

* 2.7.6 - Stripe Vendor defined fix (not in use yet) -  [Files](https://paste.laravel.io/3eb30e62-be6c-4fbf-afb5-25a3ebf54498)
* 2.7.5 - Small security update [Information](https://www.reddit.com/r/mobidoniacc/comments/qdrf13/275_security_update/) [Updated files](https://paste.laravel.io/d8fbbf22-e8a8-4504-8c64-a58fd21fe9a1)
* 2.7.4 - Admin fixes [Files](https://paste.laravel.io/d10fffcd-102e-4a1a-be41-54f15ec8035b)
* 2.7.3 - Pricing plan bug - was showing vendor currency [Files](https://paste.laravel.io/6ec88159-ad36-4ae8-8535-eb43a8372a7d)

## 2.7.0 - 2021-09-05

**Initial Version**

