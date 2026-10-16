---
sitemap: false
layout: redirect
title: Latest Version
description: You are being redirected to the latest Cuterpillar firmware version.
---
{% assign latest_version = site.versions | where: "lang", page.lang | sort: "date" | last %}{{ latest_version.url }}
