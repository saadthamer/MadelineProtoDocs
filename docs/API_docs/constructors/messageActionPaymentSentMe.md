---
title: messageActionPaymentSentMe
description: messageActionPaymentSentMe attributes, type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: messageActionPaymentSentMe  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|currency|[string](../types/string.md) | Yes|
|total\_amount|[long](../types/long.md) | Yes|
|payload|[bytes](../types/bytes.md) | Yes|
|info|[PaymentRequestedInfo](../types/PaymentRequestedInfo.md) | Optional|
|shipping\_option\_id|[string](../types/string.md) | Optional|
|charge|[PaymentCharge](../types/PaymentCharge.md) | Yes|



### Type: [MessageAction](../types/MessageAction.md)


### Example:

```
$messageActionPaymentSentMe = ['_' => 'messageActionPaymentSentMe', 'currency' => 'string', 'total_amount' => long, 'payload' => 'bytes', 'info' => PaymentRequestedInfo, 'shipping_option_id' => 'string', 'charge' => PaymentCharge];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "messageActionPaymentSentMe", "currency": "string", "total_amount": long, "payload": {"_": "bytes", "bytes":"base64 encoded bytes"}, "info": PaymentRequestedInfo, "shipping_option_id": "string", "charge": PaymentCharge}
```


Or, if you're into Lua:  


```
messageActionPaymentSentMe={_='messageActionPaymentSentMe', currency='string', total_amount=long, payload='bytes', info=PaymentRequestedInfo, shipping_option_id='string', charge=PaymentCharge}

```


