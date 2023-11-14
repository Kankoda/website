---
title: EmojiKit - Localization
hero-emoji: 🇸🇪
description: EmojiKit supports localization for all emojis and locales.
---


## Emoji Localization

[EmojiKit](/emojikit) supports emoji localization, for instance:

```swift
Emoji("😀").localizedName                   // Grinning Face
Emoji("😀").localizedName(for: .english)    // Grinning Face
Emoji("😀").localizedName(for: .swedish)    // Leende Ansikte
```

This feature uses [emoji unicode information](/emojikit/features/emoji) to generate a localization key for each emoji, which is used to resolve a localized name for each emoji.


## Limited Support

Full emoji localization is currently only implemented in English, but can be implemented on-demand for any product that needs more support.

You can [reach out]({{site.email_url}}) to help out with localization, to get a considerable discount on an SDK license.
