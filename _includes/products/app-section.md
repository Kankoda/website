Kankoda sells apps on the [App Store]({{site.appstore_url}}). Due to the main focus on SDKs, open-source and client work, most of these apps are small, but they're all built with the latest versions of [Swift]({{site.swift}}) and [SwiftUI]({{site.swiftui}}).

{% assign products = site.data.products | where:"info.app",1 %}
{% include kankoda/grids/grid.html items=products type="icons" %}