---
title: recentMeUrlChatInvite
description: recentMeUrlChatInvite attributes, type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: recentMeUrlChatInvite  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|url|[string](../types/string.md) | Yes|
|chat\_invite|[ChatInvite](../types/ChatInvite.md) | Optional|



### Type: [RecentMeUrl](../types/RecentMeUrl.md)


### Example:

```
$recentMeUrlChatInvite = ['_' => 'recentMeUrlChatInvite', 'url' => 'string', 'chat_invite' => ChatInvite];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "recentMeUrlChatInvite", "url": "string", "chat_invite": ChatInvite}
```


Or, if you're into Lua:  


```
recentMeUrlChatInvite={_='recentMeUrlChatInvite', url='string', chat_invite=ChatInvite}

```


