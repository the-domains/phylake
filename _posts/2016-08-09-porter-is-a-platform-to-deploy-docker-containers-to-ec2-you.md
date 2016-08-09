---
inFeed: true
hasPage: true
inNav: false
inLanguage: null
keywords: []
description: >-
  porter is a platform to deploy Docker containers to EC2. You might ask, "isn't
  that what ECS does?". Not quite.
datePublished: '2016-08-09T15:48:37.194Z'
dateModified: '2016-08-09T15:47:15.626Z'
title: ''
author: []
via: {}
authors: []
publisher: {}
starred: false
sourcePath: >-
  _posts/2016-08-09-porter-is-a-platform-to-deploy-docker-containers-to-ec2-you.md
url: porter-is-a-platform-to-deploy-docker-containers-to-ec2-you/index.html
_type: Article

---
# Announcing porter
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/ae79d1c7-7600-4a84-ab86-a7b2f2ff0da0.jpg)

porter is a platform to deploy Docker containers to EC2\. You might ask, "isn't that what ECS does?". Not quite.

## Why porter \[at Adobe\]

porter solved some very common problems in Adobe. The topology and needs of a microservice are largely undifferentiated yet teams were doing a lot of undifferentiated heavy lifting to get them deployed. Things like

* Setting up, configuring and maintaining CI/CD boxes
* Maintaining shared integration environments (e.g. QA2)
* Blue-green deployment
* Implementing security best practices
* Secrets management
* Internal Adobe integrations
* Provisioning AMIs with Configuration Management tools like Chef, and then baking them for use in their next deploy

All of the above were repeated with various levels of quality and automation across teams and none of them are value-added tasks.

Finally, some of Adobe's services pre-date ECS and VPC. Further complicating things - other services had strict compliance requirements that required dedicated infrastructure and strict isolation from multi-tenant environments.

## Porter is

It solved a lot of problems Adobe services needed solved by being the first to take the minimum set of requirements of a microservice and let service teams layer in the rest.