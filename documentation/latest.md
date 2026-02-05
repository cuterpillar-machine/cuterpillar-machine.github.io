---
layout: redirect
title: Latest Documentation
description: You are being redirected to the latest documentation for Cuterpillar machine.
---
{% assign latest_documentation = site.documentations | sort: "date" | last %}{{ latest_documentation.url }}