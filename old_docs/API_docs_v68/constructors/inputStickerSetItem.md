---
title: inputStickerSetItem
description: inputStickerSetItem attributes, type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputStickerSetItem  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|document|[MessageMedia, Message, Update or InputDocument](../types/InputDocument.md) | Optional|
|emoji|[string](../types/string.md) | Yes|
|mask\_coords|[MaskCoords](../types/MaskCoords.md) | Optional|



### Type: [InputStickerSetItem](../types/InputStickerSetItem.md)


### Example:

```
$inputStickerSetItem = ['_' => 'inputStickerSetItem', 'document' => InputDocument, 'emoji' => 'string', 'mask_coords' => MaskCoords];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "inputStickerSetItem", "document": InputDocument, "emoji": "string", "mask_coords": MaskCoords}
```


Or, if you're into Lua:  


```
inputStickerSetItem={_='inputStickerSetItem', document=InputDocument, emoji='string', mask_coords=MaskCoords}

```


