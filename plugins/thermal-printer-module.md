---
description: Learn how to setup the thermal Printer Module
---

# Thermal Printer Module

### Install

After you have downloaded the code from CodeCanyon, log in to your admin panel as admin and go to the "Apps" section. there is an "Add" button where you can upload the zip file you got from CodeCanyon.

{% page-ref page="how-to-install-plugin.md" %}

### Setup as project admin

After the module is installed, if you go to "Settings-&gt;Apps" you will see the "PrintNode" section. 

![](https://i.imgur.com/zi2M6jc.png)

There you should enter the "Convert API" secret.  [https://www.convertapi.com/](https://www.convertapi.com/)

Convert API is used for invoice to pdf creation in runtime. This setup is optional. 

### Setup as vendor

When vendors go to their management site \( or you as admin to the restaurant setup \), in the apps section they will be able to set up Print Node \( [https://www.printnode.com/en](https://www.printnode.com/en) \). Print Node allows us to connect any printer to the Platform with the PrintNode Client and an easy-to-use JSON API. 

![](https://i.imgur.com/EVgFW9P.png)

#### Create an account in Print Node and get PrintNode API Key

Create an account in [PrintNode.com](https://app.printnode.com/app/login/register) and choose your desired pricing. You can start free. 

![](https://i.imgur.com/vVk8cQC.png)

Enter the API Key in the Prinit Node API Key fields. 

#### Obtain a printer id

1. Download the [client](https://www.printnode.com/en/download) from PrintNode.com.
2. Install the client and login with your user and pass. 
3. Your  printer should be connected and on power 
4. Print node wll assign your printers an ID. 
5. Copy the printer ID and entere the ID in Main Thermal or Kitchen Thermal or Standard Printer ID. 
6. Setup when you want the order to be printed out

![](https://i.imgur.com/Q44ftGJ.png)

This video may help

{% embed url="https://www.youtube.com/watch?v=GIq8W5tbx6M" %}

### 

### Supported Thermal Printers

List of Supported Printers [here](https://mobidonia.com/2021/04/08/esc-pos-with-raw-printing-in-printnode/).

But I will encourage you to first test in the demo.

### Demo

In order to experience the demo, and test on an existing printer that you may have.

1. Create account in [PrintNode.com](https://printnode.com/) and download their [client](https://www.printnode.com/en/download)
2. Get the ID of your Thermal or Standard Printer \( As I do in the video \)
3. Get an API key
4. Go inside the demo of [FoodTiger](https://foodtiger.site/),[ POS Cloud](https://zebra-qr.com/), or [WhatsApp food](https://whatsappmenus.com/) and login as [admin@example.com](mailto:admin@example.com) \| secret
5. Then go to restaurants, and choose some of the demo restaurants
6. Enter your API key and Printer ID
7. Do a demo order for that restaurant
8. You should get the order prined on your printer
9. Remove the printer id and the API key from the demo site
10. Delete the API key from PrintNodel.com

 





