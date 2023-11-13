---
title: EmojiKit - Localization
layout: page
permalink: /emojikit/features/localization

hero-emoji: 🇸🇪
image:  /assets/headers/emojikit.png
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

Full emoji localization is currently only implemented to English, but can be implemented on-demand for any product that needs more support.

You can also [reach out]({{site.email_url}}) to help out with localization, to get a considerable discount on an SDK license.
