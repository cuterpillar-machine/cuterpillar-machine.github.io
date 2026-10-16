---
sitemap: false
layout: redirect
title: Остання документація
description: Перенаправлення на документацію до останньої версії Cuterpillar.
---
{% assign latest_version = site.versions | where: "lang", page.lang | sort: "date" | last %}{% assign latest_documentation = site.documentations | where: "lang", page.lang | where: "version", latest_version.version | first %}{{ latest_documentation.url }}
