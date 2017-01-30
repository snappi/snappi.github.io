---
layout: default
title: search
parent: cli
order: 0
permalink: /docs/cli/search/
---

# Searching for services

Search the registry for packages matching the search terms. If a search term starts with a /, then it's interpreted as 
a regular expression (note that many regular expression characters must be escaped or quoted in most shells).

```
$ snappi search [search terms...]
```

### Sample output
```
$ snappi search uuid
snappi WARN Building the local index for the first time, please be patient
NAME                      | DESCRIPTION           | AUTHOR          | DATE       | VERSION  | KEYWORDS                                                   
adamvr-meteor-random      | Meteor's Random…      | =adamvr         | 2015-12-10 | 0.0.4    | random meteor crypto api key generator api keys tokens UUID
an-uuid                   | Fast UUID v4…         | =warehouse13    | 2016-11-25 | 1.0.2    | uuid
angular-uid               | Creating unique IDs…  | =huei90         | 2014-05-18 | 0.1.1    | guid uuid uid angularjs angular uid
angular-uuid              | An AngularJS…         | =munkychop      | 2016-08-11 | 0.0.4    | angular angularjs angular-uuid uuid guid rfc4122 javascript libr
angular-uuid-secure       | Most secure uuid…     | =gdi2290        | 2015-05-27 | 0.0.6    | Patrick PatrickJS gdi2290 uuid $uuid ngUUID ngUUIDSecure ngUuid 
angular-uuid-service      | angular-uuid-service… | =daniellmb      | 2015-04-03 | 0.1.0    | micro service angular uuid guid generator service
⸨░░░░░░░░░░░░░░░░░░⸩ ⠴ : searching
```