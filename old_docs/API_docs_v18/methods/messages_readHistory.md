---
title: messages.readHistory
description: Mark messages as read
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.readHistory  
[Back to methods index](index.md)


Mark messages as read

### Parameters:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Optional|Where to mark messages as read|
|max\_id|[int](../types/int.md) | Yes|Maximum message ID to mark as read|
|offset|[int](../types/int.md) | Yes|Offset|
|read\_contents|[Bool](../types/Bool.md) | Yes|Mark messages as read?|


### Return type: [messages\_AffectedHistory](../types/messages_AffectedHistory.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_AffectedHistory = $MadelineProto->messages->readHistory(['peer' => InputPeer, 'max_id' => int, 'offset' => int, 'read_contents' => Bool, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.readHistory`

Parameters:

peer - Json encoded InputPeer

max_id - Json encoded int

offset - Json encoded int

read_contents - Json encoded Bool




Or, if you're into Lua:

```
messages_AffectedHistory = messages.readHistory({peer=InputPeer, max_id=int, offset=int, read_contents=Bool, })
```

### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|PEER_ID_INVALID|The provided peer id is invalid|
|Timeout|A timeout occurred while fetching data from the bot|


