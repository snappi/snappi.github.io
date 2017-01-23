---
layout: default
title: search
parent: cli
order: 2
permalink: /docs/cli/search/
---

# Searching for services

Search the registry for packages matching the search terms. If a search term starts with a /, then it's interpreted as 
a regular expression (note that many regular expression characters must be escaped or quoted in most shells).

```
$ snappi search [search terms...]
```