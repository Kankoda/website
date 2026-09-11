---
title: MediaKit

image: /assets/sdks/mediakit/header.jpg

redirect_from: /mediakit

description: MediaKit lets you create modern streaming media apps with SwiftUI on all major Apple platforms.

about: MediaKit has a rich set of models, views, and utilities, to get you up and running in no time. Build content-rich apps with list, grids, shelves, lazy loading, and powerful media tools.

features: 
  title: Powerful Media Management
  columns: 3
  items:
    - icon: lucide:box
      title: Models
      url: /sdks/mediakit/features
      text: Pre-defined media models that describe movies, shows, and collections.
    - icon: lucide:layout-template
      title: Views
      url: /sdks/mediakit/features
      text: Ready-made SwiftUI views that render your media on every platform.
    - icon: lucide:layout-grid
      title: Grids & Shelves
      url: /sdks/mediakit/features
      text: Build content-rich browse screens with grids and scrolling shelves.
    - icon: lucide:infinity
      title: Pagination
      url: /sdks/mediakit/features
      text: Lazy load large media catalogs as the user keeps scrolling.
    - icon: lucide:play
      title: Video Player
      url: /sdks/mediakit/features
      text: A full video player that drops straight into your SwiftUI views.
    - icon: lucide:wrench
      title: Video Utilities
      url: /sdks/mediakit/features
      text: Video splash screens, synced progress, and Chromecast support.
---

{% assign tiers = site.data.tiers.mediakit %}

<section class="showcase gold">
  <a name="pricing"></a>
  <article class="wide wrapper slide-in">
    <h2>Pricing</h2>
    <p>MediaKit is currently in private beta. <a href="{{site.urls.email}}">Contact us</a> if you want to give it a try.</p>
  </article>
</section>

<section class="showcase blue">
  <a name="feature-table"></a>
  <article class="wide wrapper slide-in">
    <h2>Full Feature Comparison</h2>
    <p>Compare all features across all plans.</p>
    {% include licenses/mediakit-feature-table tiers=tiers %}
  </article>
</section>