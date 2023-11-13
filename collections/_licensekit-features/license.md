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

LicenseKit uses a ``LicenseEngine`` to resolve product licenses, then perform an initial license validation to see that the license hasn't expired, and that is can be used with the current software and platform.



## License Validation

A license can validate a bunch of things. The standard ``validate()`` checks that the license is valid for the current bundle, platform and date, but there are many other validation functions as well.

If the license key or retrieved license is invalid, the license engine throws a ``LicenseError``. LicenseKit uses the same logic to validate your license when you create a license engine with your license key.



## License Information

A license contains a lot of optional information, such as the license key, the name of the product and customer, activation and expiration dates, etc. 

Most information is optional, which means that you only have to use what matters to your product.


### Customers

A license customer represents a license owner and can define things like the name, address, contact information, etc.


### Tier

A license tier defines the level of service that a specific license has access to. LicenseKit defines many standard tiers, like `.standard`, `.basic`, `.silver` and `.gold`. You can also define custom tiers.


### Platforms

A license platform defines hardware platforms that a license is valid for. This means that you can have different license prices for the number of platforms a license supports.


### Environments

A license environment defines environments that a license can be valid for. This means that you can have different license prices for the number of environments a license supports.


### Features

A license feature can be applied to various types and functions. This means that you can have different license prices for the number of features a license supports.


## Documentation

See the [LicenseKit repository]({{product.github}}) and the online documentation for more information about LicenseKit and its license model capabilities.