+++
date = "2018-03-09"
title = "Similar URL Finder"
tags = ["URLs", "Searching"]
author = "Floyd Hightower"
description = "This playbook redirects you to a browse screen view of all URL Indicators with the same URL path and query strings. It is triggered with a user action."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/similar-url-finder"
+++

## Documentation

### Triggers

- UserAction

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **errorPrefix:** `[Similar URL Finder]:`
- **redirectLink:** `#App:12145:baseTCUrl!String/auth/browse/index.xhtml?filters=typeName%20in%20(%22URL%22)%20and%20summary%20contains%20%22#App:12141:encode_url.output!String%22&intelType=indicators&owners=5`
