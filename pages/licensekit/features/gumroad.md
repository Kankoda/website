---
id: gumroad
title: Gumroad Licenses
layout: licensekit-feature
permalink: /licensekit/features/gumroad

hero: /assets/heros/licensekit/gumroad.png

description: LicenseKit lets you validate Gumroad licenses.

gumroad: https://gumroad.com
---

[LicenseKit's](/licensekit) Gumroad license service makes it super simple to validate licenses that you've sold at Gumroad, and maps the API response to a valid LicenseKit license.


## How does it work?

LicenseKit has a Gumroad license service that can fetch licenses from the Gumroad validation API. All you have to do is to provide the service with your Gumroad product ID and an optional mapper.

The response mapper provides you with a response object and a suggested LicenseKit license. You can return the standard license or map the response to a custom license whenever needed.


## Offline mode

If your software needs to work offline, LicenseKit can cache the last fetched license and ignore any non-license errors that occur during the license validation.


## License expiration

You can easily map expiration information from the Gumroad licemse, or as easily customize the expiration if you don't want to use the information provided by the service provider.