---
title: EmojiKit - Categories
layout: page
permalink: /emojikit/features/categories

hero-emoji: 🐻
image:  /assets/headers/emojikit.png
description: EmojiKit defines all emoji categories and their emojis.
---


## Emoji Categories

[EmojiKit](/emojikit) has an ``Emoji.Category`` enum that defines all emoji categories and their emojis, for instance:

```swift
try Emojis.Category.smileys.emojis  // 😀😃😄😁😆🥹😅😂...
try Emojis.Category.animals.emojis  // 🐶🐱🐭🐹🐰🦊🐻🐼...
```

You can use ``Emoji.Category.all`` to get a list of all available categories:

```swift
Emojis.Category.all     // [.frequent, .smileys, .animals, ...]
```

Categories use [Emoji version information](/emojikit/features/version-info) to filter out emojis that are unavailable to the runtime. 

This means that apps and libraries that use EmojiKit will only show emojis that are available to the device's operating system.