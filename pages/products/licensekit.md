---
id: licensekit
title: LicenseKit
layout: page
permalink: /licensekit

redirect_from: /licensekit/features

image:  /assets/headers/licensekit.png
hero: /assets/icons/licensekit.png

description: LicenseKit is a powerful license SDK for all major Apple platforms.
---

{% include kankoda/buttons/cta.html url="#pricing" %}
{% assign product=site.data.products.licensekit %}

LicenseKit helps you protect your software with commercial licenses on all major Apple platforms (iOS, iPadOS, macOS, tvOS and watchOS).


{% include kankoda/licenses/feature-section.html features=product.features %}


## Integrates with

<p class="grid integrations">
  <a href="features/gumroad">
    <img src="/assets/headers/gumroad.png" alt="LicenseKit integrates with Gumroad" title="Gumroad" />
  </a>
  <a href="features/api-licenses">
    <img src="/assets/headers/licensekit-api.png" alt="LicenseKit integrates with any REST-based license API" />
  </a>
</p>


{% include kankoda/paper/hr.md %}

{% include kankoda/licenses/pricing-section.html product=product %}
{% include kankoda/licenses/pricing-links.html  %}
{% include products/licensekit/feature-table.html tiers=product.tiers price="yearly" script=true %}
{% include products/licensekit/feature-table.html tiers=product.tiers price="monthly" script=false %}

{% include products/product-footer.md %}