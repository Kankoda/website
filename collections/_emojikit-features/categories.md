---
title: Categories
hero-emoji: 🐻 🍔 🏬
description: EmojiKit defines all emoji categories and their emojis
---


## Categories

[EmojiKit](/emojikit) has an ``Emoji.Category`` enum that defines all emoji categories and their emojis, such as:

```swift
try Emoji.Category.smileys.emojis  // 😀😃😄😁😆🥹😅😂...
try Emoji.Category.animals.emojis  // 🐶🐱🐭🐹🐰🦊🐻🐼...
```

You can use ``Emoji.Category.all`` to get a list of all available categories:

```swift
Emoji.Category.all     // [.frequent, .smileys, .animals, ...]
```

Categories use [Emoji version information](/emojikit/features/version-info) to filter out emojis that are unavailable to the runtime. 

This means that apps and libraries that use EmojiKit will only show emojis that are available to the device's operating system.