---
id: cloud
title: API/Cloud-based Licenses
layout: licensekit-feature
permalink: /licensekit/features/api-licenses

hero: /assets/heros/licensekit/api.png

description: LicenseKit lets you validate licenses with API-based requests.
---

[LicenseKit's](/licensekit) API-based license validation is a great alternative when you want to fetch and validate licenses from any external license service provider, using regular network requests.


## How does it work?

LicenseKit has an API license service that can fetch licenses from any external API. All you have to do is to provide the service a configuration and a response mapper that maps responses to licenses.

The response mapper will provide you with a strongly typed response object. You can then map the response response to a LicenseKit license, which will be validated as normal.


## Offline mode

If your software needs to work offline, LicenseKit can cache the last fetched license and ignore any non-license errors that occur during the license validation.


## License expiration

You can easily map expiration information from the service provider response, or as easily customize the expiration if you don't want to use the information provided by the service provider.