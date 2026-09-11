---
title: LicenseKit

image: /assets/sdks/licensekit/header.jpg

redirect_from: /licensekit

description: LicenseKit lets you protect your apps and SDKs with commercial licenses on all major Apple platforms.

about: LicenseKit can protect your apps and SDKs with commercial licenses, and makes it easy to verify that people have the right to use your software.

features: 
  title: Powerful License Management
  columns: 3
  items:
    - icon: lucide:circle-check
      title: License Validation
      url: /sdks/licensekit/license-validation
      text: Validate licenses in many different ways.
    - icon: lucide:binary
      title: Binary/CSV Licenses
      url: /sdks/licensekit/licenses
      text: Compile licenses into your binary.
    - icon: lucide:file-text
      title: Encrypted License Files
      url: /sdks/licensekit/licenses
      text: Create and read encrypted license files.
    - icon: lucide:cloud-lightning
      title: Integrations
      url: /sdks/licensekit/licenses
      text: Integrate with 3rd party services.
    - icon: lucide:database
      title: License Caching
      url: /sdks/licensekit/license-validation
      text: Cache the last successful validation.
    - icon: lucide:settings
      title: Service Composition
      url: /sdks/licensekit/licenses
      text: Compose services into powerful combos.
---

{% assign tiers = site.data.tiers.licensekit %}

<section class="showcase gold">
  <a name="pricing"></a>
  <article class="wide wrapper slide-in">
    {% include kankoda/licenses/pricing-title name=page.title %}
    {% include kankoda/licenses/tier-price-toggle %}
    {% include kankoda/licenses/tier-boxes tiers=sdk.tiers %}
    {% include kankoda/licenses/business-disclaimer %}
  </article>
</section>

<section class="showcase blue">
  <a name="feature-table"></a>
  <article class="wide wrapper slide-in">
    <h2>Full Feature Comparison</h2>
    <p>Compare all features across all plans.</p>
    {% include licenses/licensekit-feature-table tiers=tiers %}
  </article>
</section>