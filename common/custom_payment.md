# Custom Payment Methods

![graph](https://i.imgur.com/R56RXlt.jpg)

We have simplified the ordering process as much as we could, so you or we can be able to extend it with new payment gateways. 

The part, "Prepare Redirect link", is the crucial part of your custome payment method. It need to give the project back, a url where the customer can fulfill the purchase. 

## Create a trait
Create or copy existing trait in app/Traits/Payments. ex hasPayX.php
<img src="https://i.imgur.com/F4h3Ona.png" alt="drawing" width="200"/>

The trait should have the following methods

- paymentRules - the validation rules
- payOrder - returns validator,  and sets url of the payment. Check HasMollie.php for example.
