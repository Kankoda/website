---
id: licensekit
title: LicenseKit
layout: page
permalink: /sdks/licensekit

redirect_from: /licensekit

image:  /assets/headers/licensekit.png
hero: /assets/icons/licensekit.png

description: EmojiKit is a powerful Swift SDK for software licenses on all Apple platforms
---

{% assign product=site.data.products.licensekit %}

{% include products/sdk-section-links.md %}

LicenseKit helps you protect your Swift-based apps and SDKs with commercial licenses on all major Apple platforms (iOS, iPadOS, macOS, tvOS and watchOS).

{% include products/github-section.md %}
{% include kankoda/licenses/feature-section.html features=product.features %}
{% include kankoda/paper/hr.md %}

{% include kankoda/licenses/pricing-section.html product=product %}
{% include kankoda/licenses/pricing-links.html  %}
{% include products/feature-table-licensekit.html tiers=product.tiers price="yearly" script=true %}
{% include products/feature-table-licensekit.html tiers=product.tiers price="monthly" script=false %}

{% include products/sdk-footer.md %}