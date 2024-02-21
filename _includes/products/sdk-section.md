Kankoda has commercial, closed-source SDKs that are hosted on [GitHub]({{site.github_url}}), distributed with the [Swift Package Manager]({{site.spm}}) and sold through [Gumroad]({{site.gumroad_url}}), where each purchase generates a license key.

{% assign products = site.data.products | where:"info.sdk",1 %}
{% include kankoda/grids/grid.html items=products type="icons" %}