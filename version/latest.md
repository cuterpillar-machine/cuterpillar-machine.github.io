---
layout: redirect
title: Latest Version
description: You are being redirected to the latest release version of Cuterpillar machine.
---
{% assign latest_version = site.versions | sort: "date" | last %}{{ latest_version.url }}