# Mail server

## Why I need it

You will need to have SMTP \( way to send mail \) because the system will use it to

* Send password reset email
* Order related notifications 
* Restaurant owner registration
* Driver registration

#### SMTP from shared hosting

This is probably the easiest way to obtain SMTP data. Create an email in your hosting and get note of the credentials. You will need them in the install process.

![](https://i.imgur.com/t9Awl7B.png)

Then click on "Connect Device". You will find all required info there

![](https://i.imgur.com/QPpwKY2.png)

Here are some examples how it may look

{% tabs %}
{% tab title="SSL" %}
```text
MAIL_MAILER=sendmail
MAIL_ENCRYPTION=ssl
MAIL_PORT=465
MAIL_HOST=mail.restoqr.online
MAIL_USERNAME=themail@domain.com
MAIL_PASSWORD=*****
MAIL_FROM_ADDRESS=themail@domain.com
MAIL_FROM_NAME="${APP_NAME}"
```
{% endtab %}

{% tab title="Regular" %}
```text
MAIL_MAILER=smtp
MAIL_ENCRYPTION=null
MAIL_PORT=26
MAIL_HOST=mail.restoqr.online
MAIL_USERNAME=themail@domain.com
MAIL_PASSWORD=*****
MAIL_FROM_ADDRESS=themail@domain.com
MAIL_FROM_NAME="${APP_NAME}"
```
{% endtab %}

{% tab title="Regular 587" %}
```text
MAIL_MAILER=smtp
MAIL_ENCRYPTION=''
MAIL_PORT=26
MAIL_HOST=mail.restoqr.online
MAIL_USERNAME=themail@domain.com
MAIL_PASSWORD=*****
MAIL_FROM_ADDRESS=themail@domain.com
MAIL_FROM_NAME="${APP_NAME}"
```
{% endtab %}
{% endtabs %}

#### 3rd Party SMTP providers like SendGrid

SendGrid is the leading SMTP provider. Easy to set up and reliable service.

Get an account [here](https://sendgrid.com/).

[This article](https://sendgrid.com/docs/API_Reference/SMTP_API/integrating_with_the_smtp_api.html) is important in order to setup your SendGrid SMTP correct.

**Required**: You need to Authenticate your domain to send emails from. [Here](https://sendgrid.com/docs/ui/account-and-settings/how-to-set-up-domain-authentication/) is how.

### Test your SMTP

{% embed url="https://www.smtper.net/" caption="" %}

```text
MAIL_MAILER=smtp
MAIL_HOST=smtp.sendgrid.net
MAIL_PORT=587
MAIL_USERNAME=apikey
MAIL_PASSWORD=xxxxxxxxxxxxxxxxx
MAIL_ENCRYPTION=null

MAIL_FROM_ADDRESS='youremail@yourdomain.com'
MAIL_FROM_NAME='Your Project name'
```

