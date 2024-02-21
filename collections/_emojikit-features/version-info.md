---
title: Emoji Versions
hero-emoji: 📦
description: EmojiKit defines emoji versions and their emojis
---


## Emoji Version Information

[EmojiKit](/emojikit) has an ``Emoji.Version`` type that defines Emoji versions, with information about platform and OS availability, as well as included emojis.

To get the latest available emoji version for the current runtime, you can use ``Emoji.Version.current``:

```swift
let version = Emoji.Version.current
version.version  // 15.0
version.iOS      // 16.4
version.macOS    // 13.3
version.tvOS     // 16.4
version.watchOS  // 9.4
```

You can also request specific emoji versions, for instance:

```swift
let v15 = Emoji.Version.v15
let v14 = Emoji.Version.v14
let v13 = Emoji.Version.v13
```

You can also get the emoji version supported by a certain OS version, for instance:

```swift
let version = Emoji.Version(iOS: 15.4)
version.version  // 14.0

let version = Emoji.Version(macOS: 11.1)
version.version  // 13.0
```

This lets you figure out exactly which version you can use for a certain OS and platform version.


## Version Information

An emoji version defines in which OS versions it became available:

```swift
let version = Emoji.Version.v15
version.version  // 15.0
version.iOS      // 16.4
version.macOS    // 13.3
version.tvOS     // 16.4
version.watchOS  // 9.4
```

Emoji versions also define all older and later emoji versions:

```swift
let version = Emoji.Version.v14
version.laterVersions     // [.v15]
version.olderVersions     // [.v13_1, .v13, .v12_1, ...]
```

This information can be used in many ways, for instance to determine OS and platform availability.


## Version Emojis

An emoji version defines all emojis that were introduced in that particular versions:

```swift
let version = Emoji.Version.v14
version.emojis            // 🫠🫢🫣🫡🫥🫤🥹...
version.laterVersions     // [.v15]
version.olderVersions     // [.v13_1, .v13, .v12_1, ...]
```

Emoji versions use later versions to provide a list of emojis that were introduced in later versions:

```swift
version.unavailableEmojis // 🫨🫸🫷🪿🫎🪼🫏🪽...
```

This information can be used to filter out unavailable emojis, to avoid empty gaps in OS and platform versions where the emojis are missing.