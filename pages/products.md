---
id: products
title: Products
layout: page
permalink: /products

hero: /assets/heros/products.png

description: Kankoda builds closed-source, licence-based SDKs and commercial apps.
---

Kankoda builds closed-source, licence-based SDKs and commercial apps using [Swift]({{site.swift}}), [SwiftUI]({{site.swiftui}}) and the [Swift Package Manager]({{site.spm}}).


## SDKs

Kankoda has commercial, closed-source SDKs that are hosted on [GitHub]({{site.github_url}}), distributed with the [Swift Package Manager]({{site.spm}}) and sold through [Gumroad]({{site.gumroad_url}}), where each purchase generates a license key.

{% assign products = site.data.products | where:"info.sdk",1 %}
{% include kankoda/grids/grid.html items=products type="icons" %}


## Apps

Kankoda sells apps on the [App Store]({{site.appstore_url}}). Due to the main focus on SDKs, open-source and client work, most of these apps are small, but they're all built with the latest versions of [Swift]({{site.swift}}) and [SwiftUI]({{site.swiftui}}).

{% assign products = site.data.products | where:"info.app",1 %}
{% include kankoda/grids/grid.html items=products type="icons" %}


## Contact

Whether you build apps or complex, distributed software, Kankoda can help. Just [reach out](mailto:{{site.email}}) if you want to build something great from scratch, or need help with your apps and products.