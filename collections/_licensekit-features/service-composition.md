---
title: Service Composition
hero: /assets/heros/licensekit/services.png
description: LicenseKit can compose services to create powerful combinations
---


## Service Composition

[LicenseKit](/licensekit) lets you compose services toget maximum flexibility with minimum effort. You can for instance make a service cached, or chain multiple services together with a service proxy.


## Result Caching

License caching lets you cache any license service and use the last successfully fetched license when the license validation operation throws an error when fetching the license.

All you have to do to make a license service type cached is to wrap it in `.cached(...)`, like this:

```swift
let engine = try await LicenseEngine(licenseKey: "your-key") {
    try .cached(
        service: .api<ApiLicense>(...)
    )
}
```

License can be used to make API-based license validation more robust, and not fail when the client connectivity is lost. This is optional, to let you decide if you want to support offline validation.


## Service Proxying

Service proxying lets you chain many service together, to create flexible license validations that use multiple data sources, instead of just a single one.

All you have to do is to use the `.proxy(...)` service type and provide it with a list of services:

```swift
let engine = try await LicenseEngine(licenseKey: "your-key") {
    try .proxy(
        services: [
            .binary(
                license: license,
                customerLicenses: .all
            ),
            try .gumroad(
                license: license,
                productId: "unique-product-id",
                licenseMapping { response in
                    ...
                }
            )
        ]
    )
}
```

The code above will first try to a validate license key by checking the binary licenses that are built into the binary, then validate with Gumroad over a network call.