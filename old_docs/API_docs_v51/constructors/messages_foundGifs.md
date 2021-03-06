---
title: messages.foundGifs
description: messages_foundGifs attributes, type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: messages.foundGifs  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|next\_offset|[int](../types/int.md) | Yes|
|results|Array of [FoundGif](../types/FoundGif.md) | Yes|



### Type: [messages\_FoundGifs](../types/messages_FoundGifs.md)


### Example:

```
$messages_foundGifs = ['_' => 'messages.foundGifs', 'next_offset' => int, 'results' => [FoundGif, FoundGif]];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "messages.foundGifs", "next_offset": int, "results": [FoundGif]}
```


Or, if you're into Lua:  


```
messages_foundGifs={_='messages.foundGifs', next_offset=int, results={FoundGif}}

```


