+++
date = "2018-03-05"
title = "Robtex IP and ASN Query"
tags = ["Robtex", "Enrichment", "IPs", "ASNs"]
author = "Floyd Hightower"
description = "Query <a href='https://www.robtex.com/'>Robtex</a> for an IP or ASN."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/robtex-query"
+++

This playbook was featured in a "Playbook Friday" blog: [https://threatconnect.com/blog/robtex-asn-query-ip-query/](https://threatconnect.com/blog/robtex-asn-query-ip-query/)! The blog post includes installation instructions and a gif of how to setup the playbook.

## Images

Here is a picture of the ASN Query playbook:

![](/post/playbooks/images/robtex-asn-query.png)

Here is a picture of the IP Query playbook:

![](/post/playbooks/images/robtex-ip-query.png)

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
