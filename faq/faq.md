---
description: Frequently Asked Questions (FAQs)
---

# FAQ - Technical

## Install the project in subdomain

When you want to run your project in subdomain, you need to declare this subdomain in your Settings. To do that, you will need to go to Site setting->Setup->Subdomains and add your domain there. Ex, if you want to run the project in app.domain.com.

![](https://i.imgur.com/k6uuMa2.jpg)

## How to set overnight working time

Since 2.5.2 you are able to set overnight working time just by making ex start time 08:00PM and closing time ex 02:00 PM

## Notification translation

One really common problem is that the emails is no received correctly. Password or email is missing. and here is the reason why. Please check this [video](https://www.loom.com/share/112938a8fa31418386b5ae2c8c71303b)

## Registration is not working.

This is one of the most common problems. It happens because SMTP is not correctly set up, or not set up at all. To learn how to set it up, follow this guide

{% content-ref url="../define-basics/obtain-smtp.md" %}
[obtain-smtp.md](../define-basics/obtain-smtp.md)
{% endcontent-ref %}

## How do restaurants owner register?

At the front end part of the script, you will find the form for **Registration.** . The interested restaurants will fill the form, and Restaurant/owner account will be automatically created. An email will be sent to them.

The restaurant owner will need to log in with the email and password (generated password can change if he wants on the profile page). After that, the owner can start filling the items/categories for his restaurant.

Initially, they are assigned to a free plan.

## What languages the does site works in?

The site operates in 1 language that can be defined from the .env variable.

Easy to translate to any language. All strings are in few files.

## What technology is used?

### WEB ( Storefront and Dashboard )

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

### Error on update "tmp/v2.x.x" not found

**Problem**: When you click on the update button, you get a blank screen with error 500. if you enable debug mode, you see the error directory "tmp/v2.0.x" not found.

**Cause 1**: This mostly happens because the /tmp directory is not workspace related /tmp dir

**Cause 2**: Other common reason is that there was interuption in the download process and your server has create the zip but with incorrect structure. And then when it tries to re download, gives the error.

**Solution 1**:

* Go to you cPanel
* Open File Manager
* Open .env (it is hidden - enable hidden files)
* Add the variable
* SELF\_UPDATER\_DOWNLOAD\_PATH="/home/YOUR\_WORKSPACE\_NAME/tmp/"
* Then try again to update

**Solution 2**: Please speak with you hosting provider to clear the contents ( specifically v2.x.x.zip ) of the system **tmp** folder. If you can you can do this on your own. Server restart in most cases also clears the tmp folder.

**Solution 3**:

Change the update server

Open the .env file and change the update path to different update server

* Go to you cPanel
* Open File Manager
* Open .env (it is hidden - enable hidden files)
* Add the variable
* SELF\_UPDATER\_REPO\_URL="[http://31949.s.time4vps.cloud/v2/](http://31949.s.time4vps.cloud/v2/)"

**Solution 4:**

**Important**: Backup all your project files in case somethiing goes wrong ( you can zip the files and folder )

Do all the steps in **Solution 1**

**Try to update**

Then go to your file manager /home/YOUR\_WORKSPACE\_NAME/tmp/

There you should see the files for the update extracted

Go inside the folder ex v2.7.3

Select all the files and folder and click on the move button

Move them to /public\_html (if your project is in root) or /public\_html/sitedomain.com&#x20;

### Error on update 503

**Problem**: After an update, some users experience error 503 | Service not found.

**Cause**: This mostly happens because your PHP setup doesn't have the ZIP extension enabled.

**Solution**:

You will need to enable the ZIP extension

This is the best and simplest guide we could find on how to enable the ZIP extension in cPanel

{% embed url="https://bobcares.com/blog/enable-php-zip-extension-cpanel/" %}

Also, please talk with your hosting provider on how to enable the zip extension for you.

## Update via FTP

When for some reason, the one-click update can't work, you can easily update via FTP.

We post the updated file publicly. And you can download the updates from [here](http://updates.restoqr.online/v2/).

Go inside your current version. There should be a zip file. If the zip file version, is bigger than current, there is an update for that version.

Download the zip file and extract it locally.

Connect to your FTP, and navigate to the root of it.

Drag and Drop the folders from the update to your FTP. Overwrite them.

Repeat the procedure until you see that this is the latest version.

c

![Overwrite](https://i.imgur.com/AlYBBCo.png)

## Error 500

**Problem**\
You get a white screen with Error 500 as on this screen.

![](https://i.imgur.com/HZmpG35.png)

**Reason**\
This is a general error, meaning something wrong happened in the system. And it can be from different causes. it can be a bug or misconfiguration.

**Option 1: Enable debug mode from admin**\
First, we need to see why this error happens,\
Enable debug mode, so you can see what is behind the 500 error. To do that

1. Login as admin
2. Go In **Setting**
3. Select **Setup** tab
4. Select **APP\_DEBUG**

Then try to reproduce the problem. Now, you will see a lot more information about the problem. If you do understand the message, you get, you may fix the problem on your own. Some common ones are SMTP are Stripe Misconfiguration. For these ones you may try to fix on your own, by going in settings to check if what you have entered is correct.

**Option 2: Enable debug mode from cPanel file manager**\
In case you are not able to login, you have the option to manually enable debug mode.

1. Go to your cPanel file manager
2. Find the file **.env** and edit it. This file is hidden so you may need to [show hidden file in cPanel](https://www.plothost.com/kb/show-hidden-files-htaccess-cpanel-file-manager/)
3. Locate APP\_DEBUG=false and change it to
4. APP\_DEBUG=true
5. Now you have debug mode ON

Then try to reproduce the problem. Now, you will see a lot more information about the problem. If you do understand the message, you get, you may fix the problem on your own. Some common ones are SMTP are Stripe Misconfiguration. For these ones you may try to fix on your own, by going in settings to check if what you have entered is correct.

**Share a link to the error** For some other reported errors, don't hesitate to contact us with a link of the Flare Error of the problem here [https://help.mobidonia.com/](https://help.mobidonia.com)

Here is how you can obtain a link.

![](https://i.imgur.com/pfxNCqH.png)

## Error 500 on migrating languages

**Problem**\
Before, 2.0.8 if you try to migrate language you can get an error 500. And some of the items like the categories can be translated multiple times like `{en:\\\en:\\\......}`

**Reason**\
This happens because we didn't look into object active status. And script crashed when it tried to translate an un-active record.

**Solution**\
Update to 2.0.8+ For the`{en:\\\en:\\\......}`, if you don't have a lot of data, you can manually edit them from the admin. If you have a lot of data,

* Export the categories and items table
* Find replace, so it looks normal
*   Delete categories and items by ignoring foreign keys and import again

    Or ask for help from us.

Then make the translation migration again. Now should go fine.

## SQL Error - Table not found

**Error**\
After installation, when you open your site, you see an error screen with a report similar to this.

```
local.ERROR: SQLSTATE[42S22]: Column not found: 1054 Unknown column 'plan.plan_id'
```

**Reason**\
The most common problem for this is because you have entered the wrong credentials/user/pass for the Database and the setup of the database was incomplete.

**Solution**

1. Open the file **.env** and make sure you have entered the correct DB data
2. Remove file storage/installed
3. Try to install again by visiting yourdomain.com/install

If that doesn't help, please create a ticket, and if you can share cPanel / Admin details with us so we can look into the problem.

## Error on uploading an image

**Error**

"PHP Fileinfo extension must be installed

**Reason**\
"PHP Fileinfo extension must be installed/enabled to use Intervention Image."

The project needs the [fileinfo](https://i.stack.imgur.com/vhN3E.png) extension.

**Solution**

As you can see on the [image](https://i.stack.imgur.com/vhN3E.png), it can be enabled from PHP Selector. But if there is no PHP Selector you should have access to **WHM**.

**IN WHM**

Initially, we login to WHM and navigate as follows,

Software >> EasyApache 4 >> Customize >> PHP extensions.

Here we search for **fileinfo** and enable phpx.x-php-fileinfo for all versions. Finally, we click on Review and Provision.

This enables the file extension for all the PHP websites in the server.

Let me know about this.

## How to force HTTPS

In order to force your site to run only in HTTPS login as admin, then go in "Site Setting" and in "Setup" tab locate the "App environment". And set it to "Production".

This is what can be done on the Project level. Make sure you have valid SSL and that you have set the HTTPS force on the hosting level also.

## How to enable PHP Extension

If you get an error like this one

![](https://i.imgur.com/EXp59rL.png)

This indicates that the INTL extension - or depending on the problem, another one is not enabled.

Here is a good video on how you can enable it. If you can't. Please speak with your hosting provider.

{% embed url="https://www.youtube.com/watch?v=kYwRtMwWerQ" %}

## Staff module error 500

**Problem**: you get error 500 when adding new staff member.

**Reason**: With older installs/db the "staff" role is missing

**Solution**: Manually add it in the database

![](https://i.imgur.com/y2mcVTJ.png)
