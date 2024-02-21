---
title: Skin Tones
hero-emoji: 👍🏻👍🏾👍🏿
description: EmojiKit defines emoji skin tones
---


## Skin Tone Support

[EmojiKit](/emojikit) has extensive ``Emoji`` skin tone information:

```swift
Emoji("👍").hasSkinToneVariants     // true
Emoji("🚀").hasSkinToneVariants     // false
Emoji("👍🏿").neutralSkinToneVariant  // 👍
Emoji("👍").skinToneVariants        // 👍👍🏻👍🏼👍🏽👍🏾👍🏿
Emoji("👍").skinToneVariantActions  // The above variants as keyboard actions
```

Skin tone variants will automatically be shown in a secondary callout when long pressing emojis in the library's `Emoji.Picker` component. 


## Limited support

Note that multiple skin tone components are currently not supported, such as two persons kissing.
