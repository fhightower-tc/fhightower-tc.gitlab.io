+++
date = "2019-01-04"
title = "URL Utility"
tags = ["URLs", "Utility", "Indicators", "URL Schemes", "URL Domain Names", "URL Paths", "URL Query Parameters", "URL Fragments"]
author = "Floyd Hightower"
description = "Perform operations and get data from a URL."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_URL_Utility"
+++

# URL Utility

This app can take either a single URL or a list of URLs. Given a URL or a list of URLs, this app will perform the following operations on URL indicators:

- Get the scheme(s) from the URL(s) (e.g. `https` from `https://pb-constructs.hightower.space/playbooks/` => ``)
- Get the domain name(s) from the URL(s) (`pb-constructs.hightower.space` from `https://pb-constructs.hightower.space/playbooks/`)
- Get the path(s) from the URL(s) (`/playbooks/` from `https://pb-constructs.hightower.space/playbooks/`)
- Get the query parameter(s) from the URL(s) (`q=iteration` from `https://pb-constructs.hightower.space/playbooks/?q=iteration`)
- Get the fragment(s) from the URL(s) (`example-use-case` from `https://pb-constructs.hightower.space/playbooks/constructs/array_iterator#example-use-case`)

This app also allows you to remove the query parameters, fragments, and paths from URLs.

## Release Notes

### 0.0.1

* Initial Release
