---
title: Vietnamese Input

image: /assets/sdks/vietnameseinput/header.jpg

redirect_from: /vietnameseinput

description: Vietnamese Input lets you add support for Vietnamese text input to any SwiftUI app on all major Apple platforms.

about: Vietnamese Input is easy to use and lets you get up and running in no time.

tilt-device: 0

features: 
  title: Powerful Typing Tools
  columns: 3
  items:
    - icon: lucide:keyboard
      title: Input Types
      url: /sdks/vietnameseinput/features
      text: Type Vietnamese with TELEX, VNI, and VIQR, using standard input methods.
    - icon: lucide:a-large-small
      title: Diacritics
      url: /sdks/vietnameseinput/features
      text: A complete set of Vietnamese-specific diacritics, with rich text replacements.
    - icon: lucide:play-circle
      title: Simulations
      url: /sdks/vietnameseinput/features
      text: Simulate text input to build visualizations and educational experiences.
---

{% assign tiers = site.data.tiers.vietnameseinput %}

<section class="showcase gold">
  <a name="pricing"></a>
  <article class="wide wrapper slide-in">
    {% include kankoda/licenses/pricing-title name=page.title %}
    {% include kankoda/licenses/tier-price-toggle %}
    {% include kankoda/licenses/tier-boxes tiers=tiers %}
    {% include kankoda/licenses/business-disclaimer %}
  </article>
</section>

<section class="showcase blue">
  <a name="feature-table"></a>
  <article class="wide wrapper slide-in">
    <h2>Full Feature Comparison</h2>
    <p>Compare all features across all plans.</p>
    {% include licenses/vietnameseinput-feature-table tiers=tiers %}
  </article>
</section>