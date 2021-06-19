---
description: Frequently Asked Questions (FAQs)
---

# FAQ - Technical

## How to set 24h working time

We have made an overwrite, if you set closing time to be 23:59 to be interpreted as no closing at all. 

Ex - night club working hours from 22 and closes at 4 in the morning.  
Friday - 22:00 - 23:59
Saturday - 00:00 - 04:00  | Saturday Shift 2 - 22:00 - 23:59
Sunday - 00:00 - 04:00 

## Registration is not working.

This is one of the most common problems. It happens because SMTP is not correctly set up, or not set up at all. To learn how to set it up, follow this guide

{% page-ref page="../define-basics/obtain-smtp.md" %}

## How restaurants owner register?

At the front end part of the script, you will find the form for **Registration.** . The interested restaurants will fill the form, and Restaurant/owner account will be automatically created. An email will be sent to them.

The restaurant owner will need to log in with the email and password \(generated password can change if he wants on the profile page\). After that, the owner can start filling the items/categories for his restaurant.

Initially, they are assigned to a free plan.

## What languages the does site works in?

The site operates in 1 language that can be defined from the .env variable.

Easy to translate to any language. All strings are in few files.

## What technology is used?

### WEB \( Storefront and Dashboard \)

* Laravel - PHP Framework
* MySQL Database
* Bootstrap - Based on Argon Design from Creative Tim
* React JS
* Mobile ready - Both storefront and dashboard

## How to delete the demo data?

* Login as admin
* Go to settings
* Delete demo data

## Update problems

### Error on update 500

**Problem**: When you click on the update button, you get a blank screen with error 500.

**Cause**: This mostly happens because there is not enough memory available. You can check the "Error" pages in cPanel to confirm

**Solution**:

* Go to your cPanel
* There find the tool "MultiPHP INI Editor"
* Select the project
* memory\_limit put to 512M
* This should be enough
* Then try to update again

### Error on update  "tmp/v2.0.x" not found

**Problem**: When you click on the update button, you get a blank screen with error 500. if you enable debug mode, you see the error directory "tmp/v2.0.x" not found.

**Cause**: This mostly happens because the /tmp directory is not workspace related /tmp dir

**Solution**:

* Go to you cPanel
* Open File Manager
* Open .env \(it is hidden - enable hidden files\)
* Add the variable 
* SELF\_UPDATER\_DOWNLOAD\_PATH="/home/YOUR\_WORKSPACE\_NAME/tmp/" 
* Then try again to update

### Error on update 503

**Problem**: After an update, some users experience error 503 \| Service not found.

**Cause**: This mostly happens because your PHP setup doesn't have the ZIP extension enabled.

**Solution**:

You will need to enable the ZIP extension

This is the best and simplest guide we could find on how to enable the ZIP extension in cPanel

{% embed url="https://bobcares.com/blog/enable-php-zip-extension-cpanel/" caption="" %}

Also, please talk with your hosting provider on how to enable the zip extension for you.

## Error 500

**Problem**  
You get a white screen with Error 500 as on this screen.

![](https://i.imgur.com/HZmpG35.png)

**Reason**  
This is a general error, meaning something wrong happened in the system. And it can be from different causes. it can be a bug or misconfiguration.

**Solution**  
First, we need to see why this error happens,  
Enable debug mode, so you can see what is behind the 500 error. To do that

1. Login as admin
2. Go In **Setting**
3. Select **Setup** tab
4. Select **APP\_DEBUG**

Then try to reproduce the problem. Now, you will see a lot more information about the problem. If you do understand the message, you get, you may fix the problem on your own. Some common ones are SMTP are Stripe Misconfiguration. For these ones you may try to fix on your own, by going in settings to check if what you have entered is correct.

**Share a link to the error** For some other reported errors, don't hesitate to contact us with a link of the Flare Error of the problem here [https://help.mobidonia.com/](https://help.mobidonia.com)

Here is how you can obtain a link.

![](https://i.imgur.com/pfxNCqH.png)

## Error 500 on migrating languages

**Problem**  
Before, 2.0.8 if you try to migrate language you can get an error 500. And some of the items like the categories can be translated multiple times like `{en:\\\en:\\\......}`

**Reason**  
This happens because we didn't look into object active status. And script crashed when it tried to translate an un-active record.

**Solution**  
Update to 2.0.8+ For the`{en:\\\en:\\\......}`, if you don't have a lot of data, you can manually edit them from the admin. If you have a lot of data,

* Export the categories and items table
* Find replace, so it looks normal
* Delete categories and items by ignoring foreign keys and import again

  Or ask for help from us.

Then make the translation migration again. Now should go fine.

## SQL Error - Table not found

**Error**  
After installation, when you open your site, you see an error screen with a report similar to this.

```text
local.ERROR: SQLSTATE[42S22]: Column not found: 1054 Unknown column 'plan.plan_id'
```

**Reason**  
The most common problem for this is because you have entered the wrong credentials/user/pass for the Database and the setup of the database was incomplete.

**Solution**

1. Open the file **.env** and make sure you have entered the correct  DB data
2. Remove file storage/installed
3. Try to install again by visiting yourdomain.com/install

If that doesn't help, please create a ticket, and if you can share cPanel / Admin details with us so we can look into the problem.

## Error on uploading an image

**Error**

"PHP Fileinfo extension must be installed

**Reason**  
"PHP Fileinfo extension must be installed/enabled to use Intervention Image."

The project needs the [fileinfo](https://i.stack.imgur.com/vhN3E.png) extension.

**Solution**

As you can see on the [image](https://i.stack.imgur.com/vhN3E.png), it can be enabled from PHP Selector. But if there is no PHP Selector you should have access to **WHM**.

**IN WHM**

Initially, we login to WHM and navigate as follows,

Software &gt;&gt; EasyApache 4 &gt;&gt; Customize &gt;&gt; PHP extensions.

Here we search for **fileinfo** and enable phpx.x-php-fileinfo for all versions. Finally, we click on Review and Provision.

This enables the file extension for all the PHP websites in the server.

Let me know about this.

## How to change WhatsApp Message

### Change the text
To just simply  change the text, go inside the admin area and then in Translations. 
In Translations, select the "Single" group and look for the text you want to change. 

### Change the layout
To change the content and layout or completely modify the message, open **resources/views/messages/social.blade.php**.

Here you are able to modify the complete message send on WhatsApp. 

