# Pricing Plans

## Subscription processors

At the moment we have 3 subscription processors. Stripe, PayPal and Paddle.com

You can manage the settings for them if you login as admin and then to got Settings-&gt; Finances.

## **Information about the pricing plans**

{% embed url="https://www.youtube.com/watch?v=RakPeKbQpsk" caption="" %}

### How to get the keys

**Stripe Keys**

[https://stripe.com/docs/keys](https://stripe.com/docs/keys)

**PayPal keys**

[https://developer.paypal.com/docs/api-basics/sandbox/credentials/](https://developer.paypal.com/docs/api-basics/sandbox/credentials/)

**Paddle**

Your Paddle Vendor ID can be found on the [Authentication page](https://vendors.paddle.com/authentication) in your Paddle dashboard.



### Stripe

First, login as admin, and go in Setting. Go in the Finances tab, and make sure Tool used for subscriptions is Stripe.

Just create an account in stripe and fill your stripe credentials in Settings-&gt; Finances.

One common mistake is to use plan\_id instead of price\_id. So you should use the price\_id from Stripe. As you can see in the image.

![](https://i.imgur.com/0WnONPQ.png)

### PayPal

First, login as admin, and go in Settings. Go in the Finances tab, and make sure Tool used for subscriptions is PayPal.

First you will need to create developer account on PayPal on the following [link](https://developer.paypal.com/classic-home). After you create the account open the **Dashboard** from the menu in the right upper corner.

Now select **My Apps and credentials** and click on the button **Create App**.

Now fill the informations that are required and make sure that you will select the **Merchant App Type**. After you created the app you will see the **Client ID** and **Secret** credentials **generated.** Copy them and fill your PayPal credentials in Settings-&gt; Finances. First, test in development - sandbox mode.

![](https://i.imgur.com/MIa2WGc.png)

Create account on the official [PayPal website](https://www.paypal.com/) and the login with the account.

Open this [URL](https://www.paypal.com/billing/plans) and make sure that you are logged in before you open this URL.

You will see the option for creating new plans. Create your billing plans and then fill the plans information in your admin panel \(Pricing plans\).

![](https://i.imgur.com/ptCNXWK.png)

### Paddle

QR Menu maker uses Paddle.com as payment process. It is supper easy to setup.

First, login as admin, and go in Setting. Go in the Finances tab, and make sure Tool used for subscriptions is Paddle.

Go in Paddle.com and define your pricing plans.

As admin, when you create the plan, you will have the option to set Paddle Plan id.

In Paddle Developer - WebHooks set the following web-hook to receive subscription notification

```text
https://yoursite.com/paddle
```

{% embed url="https://vendors.paddle.com/alerts-webhooks" caption="" %}

You will also need to add paddleVendorID in .env file. You can use the .env editor to achieve this. paddleVendorID can be found in your Paddle Developer Tools -&gt; Authentication.

[https://vendors.paddle.com/authentication](https://vendors.paddle.com/authentication)

```text
paddleVendorID=YOUR_PADDLE_VENDOR_ID
```

## **Payment currency**

QR Menu Maker supports many currencies. By default is set to **usd** currency but you can change into one of the [available currencies](https://stripe.com/docs/currencies#presentment-currencies). You can manage the currencies in Setting -&gt; Localization.

```text
CASHIER_CURRENCY="usd" //usd,eur etc.
```

