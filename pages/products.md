---
id: products
title: Products
layout: page
permalink: /products

hero: /assets/heros/products.png

description: Kankoda can help you build amazing commercial software. Here are some of our own products.
---

Whether you create apps, SDKs or complex, distributed software, Kankoda can help. Here are some of our own apps and license-based products.


## Gumroad

KeyboardKit sells a couple of license-based SDKs on [Gumroad]({{site.gumroad_url}}). License customers receive a license key that they can use to get access to the SDK.

{% assign products = site.data.products | where:"app",1 %}
{% include kankoda/grids/grid.html items=products link="products" type="icons" %}


## Products

KeyboardKit sells apps on the [App Store]({{site.appstore_url}}). Due to focus on client work, open-source and SDKs, most of our apps are smaller in scope.

{% assign products = site.data.products | where:"app",1 %}
{% include kankoda/grids/grid.html items=products link="products" type="icons" %}


## Contact

Don't hesitate to [reach out](mailto:{{site.email}}) if you need help with apps in particular or software in general, or if you want to build something great from scratch. 