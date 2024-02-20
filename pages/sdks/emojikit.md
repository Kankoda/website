---
id: emojikit
title: EmojiKit
layout: page
permalink: /sdks/emojikit

redirect_from: /emojikit

image:  /assets/headers/emojikit.png
hero: /assets/icons/emojikit.png

description: EmojiKit is a powerful Swift SDK with emoji features for all Apple platforms
---

{% assign product=site.data.products.emojikit %}

{% include products/sdk-section-links.md %}

EmojiKit is an emoji SDK for Swift and SwiftUI-based apps and libraries on all major Apple platforms (iOS, iPadOS, macOS, tvOS, watchOS & visionOS).

{% include products/github-section.md %}
{% include kankoda/licenses/feature-section.html features=product.features %}
{% include kankoda/paper/hr.md %}

{% include kankoda/licenses/pricing-section.html product=product %}
{% include kankoda/licenses/pricing-links.html  %}
{% include products/feature-table-emojikit.html tiers=product.tiers price="yearly" script=true %}
{% include products/feature-table-emojikit.html tiers=product.tiers price="monthly" script=false %}

{% include products/sdk-footer.md %}