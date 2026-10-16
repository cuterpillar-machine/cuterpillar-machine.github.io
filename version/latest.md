---
sitemap: false
layout: redirect
title: Остання версія
description: Перенаправлення на останню версію прошивки Cuterpillar.
---
{% assign latest_version = site.versions | where: "lang", page.lang | sort: "date" | last %}{{ latest_version.url }}
