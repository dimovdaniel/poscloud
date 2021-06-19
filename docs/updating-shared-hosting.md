---
description: >-
  This process takes around 5 min. Your site will be down. You should run it
  when you have lowest number of visitors, or put some website redirect.
---

# Updating - Shared hosting

## Video Instruction

{% embed url="https://youtu.be/-nufYtcRWmo" caption="" %}

## 1. If you have made any changes to the code

In case, you have made any changes on the code, css or js file. Backup them first so you don't lose your work. Download them or take a note of what you have changed.

### 2. Backup these files and folder in case something goes wrong

* [ ] public/uploads - here are the uploaded images \( you can zip it and move it somewhere \)
* [ ] public/byadmin - here are the custom CSS entered from the admin - if you have any
* [ ] .env \( **Required**  - Download it\)
* [ ] modified - created language files - resource/lang/YOUR\_LOCALE

### 3. Download the code from CodeCanyon and upload the zip

Download the code from CodeCanyon and directly upload it on your hosting, in the same place where your existing site is.

### 4. Extract the zip file

Extract the zip files. Overwriting old files.

### **5. Restore your .env file**

Go once again to your file manager and upload your old .env file

### 6. IMPORTANT: Let know the project that the system is already installed

Create an empty file named **installed** in **/storage**

### 7. After files are moved, open your site and go to Settings

Here, if there are migrations for the database to be done, will be run.

