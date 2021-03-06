---
layout: default
title: snappi search
parent: cli
order: 1
permalink: /cli/snappi/search/
---

# Searching for services

Search the registry for packages matching the search terms. If a search term starts with a /, then it's interpreted as 
a regular expression (note that many regular expression characters must be escaped or quoted in most shells).

```
$ snappi search <search terms...>
```

### Sample output
```sh
$ snappi search dthor
┌────────────────────┬─────────────────────────┬───────────┬─────────┬───────────┐
│ name               │ description             │ author    │ version │ keywords  │
├────────────────────┼─────────────────────────┼───────────┼─────────┼───────────┤
│ dthor-user-service │ User management service │ David Th… │ 1.0.0   │ dthor,us… │
└────────────────────┴─────────────────────────┴───────────┴─────────┴───────────┘
```