---
title: invokeWithTakeout
description: Invoke method from takeout session
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: invokeWithTakeout  
[Back to methods index](index.md)


Invoke method from takeout session

### Parameters:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|takeout\_id|[long](../types/long.md) | Yes|The takeout session ID|
|query|[!X](../types/!X.md) | Yes|The query|


### Return type: [X](../types/X.md)

### Can bots use this method: **YES**


### MadelineProto Example:


```
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$X = $MadelineProto->invokeWithTakeout(['takeout_id' => long, 'query' => !X, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - invokeWithTakeout
* params - `{"takeout_id": long, "query": !X, }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/invokeWithTakeout`

Parameters:

takeout_id - Json encoded long

query - Json encoded !X




Or, if you're into Lua:

```
X = invokeWithTakeout({takeout_id=long, query=!X, })
```

