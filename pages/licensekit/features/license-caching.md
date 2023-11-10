---
id: caching
title: License Caching
layout: page
permalink: /licensekit/features/license-caching

hero: /assets/heros/licensekit/cache.png

description: LicenseKit lets you cache any license service
---

LicenseKit lets you wrap any license service in a cached service and use the last successful validation if an error occurs while validating the license.


## How does it work?

A cached license service is just a service that takes another service as input when you create it. It will then use that services to fetch licenses.

The cached service will then save the last license for any given licsense key, and return that license if the validation fails due to any other error than a license validation error.

This can be used to easily make API-based license validation more robust, and not fail when the client connectivity is lost.