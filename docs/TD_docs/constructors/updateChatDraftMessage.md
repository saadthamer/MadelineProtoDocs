---
title: updateChatDraftMessage
description: Chat draft has changed. Be aware that the update may come in the currently open chat with the old content of the draft. If the user has changed the content of the draft, the update shouldn't be applied
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: updateChatDraftMessage  
[Back to constructors index](index.md)



Chat draft has changed. Be aware that the update may come in the currently open chat with the old content of the draft. If the user has changed the content of the draft, the update shouldn't be applied

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|chat\_id|[int53](../types/int53.md) | Yes|Chat identifier|
|draft\_message|[draftMessage](../constructors/draftMessage.md) | Yes|New chat draft_message, nullable|
|order|[int64](../constructors/int64.md) | Yes|New value of the chat order|



### Type: [Update](../types/Update.md)


