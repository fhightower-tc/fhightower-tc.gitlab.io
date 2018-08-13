+++
date = "2018-03-05"
title = "Cymon IP and Host Query"
tags = ["Cymon", "IPs", "Hosts", "Enrichment"]
author = "Floyd Hightower"
description = "This playbook lets you query Cymon for an IP Address or Host."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/cymon-query-ip-and-05"
+++

## Documentation

### Triggers

- UserAction

### User Variables

This playbook expects the following user variables:

- **text:** `Cymon API Token`

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **errorMessagePrefix:** `[Cymon Query PB]:`
- **address:** `ip`
- **link:** `https://cymon.io/#Trigger:1212:trg.action.item!String`
- **host:** `domain`
- **link:** `https://cymon.io/domain/#Trigger:1212:trg.action.item!String`
- **successMessage:** `This indicator is found in #App:12970:array.length!String sources: <a href="#App:12694:link!String" target="_blank">#App:12694:link!String</a>.`
- **failureMessage:** `This indicator was not found in cymon.`
