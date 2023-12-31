---
id: emojikit
title: EmojiKit
layout: page
permalink: /emojikit

redirect_from: /emojikit/features

image:  /assets/headers/emojikit.png
hero: /assets/icons/emojikit.png

description: EmojiKit is a powerful emoji SDK for all major Apple platforms.
---

{% include kankoda/buttons/cta.html url="#pricing" %}
{% assign product=site.data.products.emojikit %}

EmojiKit brings emoji power features to Swift- and SwiftUI-based apps and libraries on all major Apple platforms (iOS, iPadOS, macOS, tvOS and watchOS).


{% include kankoda/licenses/feature-section.html features=product.features %}


{% include kankoda/paper/hr.md %}

{% include kankoda/licenses/pricing-section.html product=product %}
{% include kankoda/licenses/pricing-links.html  %}
{% include products/emojikit/feature-table.html tiers=product.tiers price="yearly" script=true %}
{% include products/emojikit/feature-table.html tiers=product.tiers price="monthly" script=false %}

{% include products/sdk-footer.md %}