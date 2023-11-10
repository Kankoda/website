---
id: proxying
title: Service Proxying
layout: page
permalink: /licensekit/features/service-proxying

hero: /assets/heros/licensekit/proxy.png

description: LicenseKit lets you combine multiple service types into a single service.
---

LicenseKit lets you create service proxies that wrap many other services, to create flexible validation flows that use multiple data sources, instead of just a single one.

## How does it work?

A service proxy is just a service that takes a list of services as input when you create it. It will then use all those services to fetch licenses.

For instance, say that you have several license files. You can then create one service per file and then combine them in a service proxy that checks all files until it finds a match.