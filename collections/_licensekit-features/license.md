---
title: License Validation
hero: /assets/heros/licensekit/license.png
description: LicenseKit can validate licenses in flexible and powerful ways.
---

[LicenseKit](/licensekit) has a ``License`` that represents a software license that can be resolved with a license key.

{% include kankoda/data/product.html name="LicenseKit" %}

A license can specify and validate license expiration date, tier, customer and other information, as well as the supported platforms, bundle IDs, environments, features, and much more.

LicenseKit can use services to get licenses from the product binary, read licenses from files, fetch licenses from remote APIs, integrate with external services like Gumroad, etc.


## License Engine

LicenseKit uses a ``LicenseEngine`` to resolve licenses, then performs an initial license validation to see that the license hasn't expired, and that is can be used with the current software and platform.



## License Validation

A license can validate a bunch of things. The standard ``validate()`` function checks that the license is valid for the current bundle, platform and date, but there are many other validation types.



## License Information

A license has a lot of information, such as license key and tier, product and owner name, activation and expiration dates, etc. It can also specify valid platforms and environments, features, etc.


## Documentation

See the [GitHub repository]({{product.github}}) and online documentation for more information about the LicenseKit license model capabilities.