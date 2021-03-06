---
title: messages.report
description: Report a message
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.report  
[Back to methods index](index.md)


Report a message

### Parameters:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Optional|The user that sent the messages|
|id|Array of [int](../types/int.md) | Yes|The messages to report|
|reason|[ReportReason](../types/ReportReason.md) | Yes|The reason why you're sending this report|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **YES**


### MadelineProto Example:


```
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->messages->report(['peer' => InputPeer, 'id' => [int, int], 'reason' => ReportReason, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - messages.report
* params - `{"peer": InputPeer, "id": [int], "reason": ReportReason, }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.report`

Parameters:

peer - Json encoded InputPeer

id - Json encoded  array of int

reason - Json encoded ReportReason




Or, if you're into Lua:

```
Bool = messages.report({peer=InputPeer, id={int}, reason=ReportReason, })
```

