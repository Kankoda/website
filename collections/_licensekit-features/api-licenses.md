---
title: API/Cloud-based Licenses
hero: /assets/heros/licensekit/api.png
description: LicenseKit can validate licenses over the Internet, using any REST API
---


## API/Cloud-based licenses

[LicenseKit's](/licensekit) API-based license engine is a great alternative when validating licenses from external license providers, using regular REST API requests.


## How does it work?

LicenseKit has an API license service that can fetch licenses from any external API. All you have to do is to provide the service a configuration and a response mapper to map a response to a license.

The response mapper provides you with a strongly typed response. You can then map the response response to a LicenseKit license, which will be validated as normal.


## Offline mode

If your software needs to work offline, LicenseKit can cache the last fetched license and ignore any non-license errors that occur during the license validation.