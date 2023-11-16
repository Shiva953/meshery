---
layout: default
title: Application Management
permalink: tasks/application-management
type: tasks
language: en
list: include
---

Meshery's application management features allows you to store, manage, configure, and un/deploy your applications to any of your connected kubernetes clusters. Meshery also comes with some sample applications out-of-the-box for you to quickly get started. Separately, you can import any of applications from [Meshery Catalog](https://meshery.io/catalog).

## What is a Meshery Application?

A single file (future: which could be split into multiple files upon user request) that comprises Kubernetes objects representative of a complete set of Kubernetes workload resources. 

You can import an applications as:

- Kubernetes manifest
- Meshery Design
- Helm Charts
- Docker Compose

You can also import application files from the filesystem, a URL or from a GitHub repository.

<img src="{{ site.baseurl }}/assets/img/configuration-management/meshery-applications.png" />

See [Guide: Application Management]() for a more detailed guide on working with your applications in Meshery.

**Known Caveats:**
- Rollouts do not support custom ServiceAccount names. User's ServiceAccount name must be the same as the Rollouts name.
