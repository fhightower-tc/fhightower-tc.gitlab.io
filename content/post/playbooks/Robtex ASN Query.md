+++
date = "2018-03-05"
title = "Robtex IP and ASN Query"
tags = ["Robtex", "Enrichment", "IPs", "ASNs"]
author = "Floyd Hightower"
description = "Query [Robtex](https://www.robtex.com/) for an IP or ASN."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/robtex-query"
+++

<!-- Query [Robtex](https://www.robtex.com/) for an IP or ASN. -->

## Documentation for "Robtex ASN Query" Playbook

### Triggers

- UserAction

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **robtexAPI:** `https://freeapi.robtex.com/asquery/#App:10683:asn!String`
- **errorPrefix:** `[Robtex ASN Query]: `
- **slackChannel:** `#slack-channel`

## Documentation for "Robtex IP Query" Playbook

### Triggers

- UserAction

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **robtexAPI:** `https://freeapi.robtex.com/ipquery/#Trigger:1003:trg.action.item!String`
- **errorPrefix:** `[Robtex IP Query]: `
- **slackChannel:** `#slack-channel`
