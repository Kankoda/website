---
title: EmojiKit - Emojis
hero-emoji: 😀
description: EmojiKit lets you work with emojis in a structured way.
---


## Emoji Model

[EmojiKit](/emojikit) has an ``Emoji`` struct that lets you work with emojis in structured ways:

```swift
let emoji = Emoji("😀")
```

You can use ``Emoji.all`` to get a list of all emojis from all categories, that are available to the currently exeucting runtime:

```swift
let emojis = Emoji.all          // 😀😃😄😁😆🥹😅😂🤣🥲...
```

The ``Emoji`` type also serves as a namespace for most EmojiKit features, which means that most types are wrapped within this struct.


## Unicode Information

The `Emoji` type has unicode-specific properties that are used for identity and naming:

```swift
Emoji("👍").unicodeIdentifier   // \\N{THUMBS UP SIGN}
Emoji("👍🏿").unicodeIdentifier   // \\N{THUMBS UP SIGN}\\N{EMOJI MODIFIER FITZPATRICK TYPE-6}
Emoji("🚀").unicodeIdentifier   // \\N{ROCKET}
Emoji("👍").unicodeName         // Thumbs Up Sign
Emoji("👍🏿").unicodeName         // Thumbs Up Sign
Emoji("🚀").unicodeName         // Rocket
```

These properties have manual overrides for some emojis that lack proper information, such as flags.


## Search

The `Emoji` type supports searching for emojis that matches certain search queries:

```swift
Emoji("👍").matches("thumb")    // true
Emoji("👍🏿").matches("thumb")    // true
Emoji("🚀").matches("thumb")    // true

[Emoji("👍"), Emoji("👍🏿") Emoji("🚀")]
    .matching("thumb")          // 👍, 👍🏿
```

This can be used to quickly filter emojis in code or letting users search for specific emojis.


## Extensions

EmojiKit has String and Character extensions that can be used to detect and handle emojis:

```swift
"Hello!".containsEmoji          // false
"Hello! 👋".containsEmoji       // true
"Hello! 👋".containsOnlyEmojis  // false
"👋".containsOnlyEmojis         // true
"Hello! 👋😀".emojis            // ["👋", "😀"]
"Hello! 👋😀".emojiString       // "👋😀"
"🫸🫷".isSingleEmoji            // false
"👍".isSingleEmoji              // true
```

These extensions are used to power many features in the library, but can be used stand-alone as well.
