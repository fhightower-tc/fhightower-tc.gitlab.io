+++
date = "2018-07-23"
title = "Submit to urlscan.io"
tags = ["urlscan.io", "Hosts", "URLs", "Indicators", "Enrichment"]
author = "citadelintellgenceresearch"
description = "Submit a host or URL to urlscan.io for enrichment."
categories = ["Playbook Components"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/submit_to_urlscan"
downloadLinks = ["/post/playbook-components/downloads/Submit to urlscan.io.pbx"]
+++

This component parses out associated IP addresses, file hashes, hosts, and URLs. Additionally, urlscan.io takes a screenshot of the page as well as grabs the source code of the page. The URLs linking to the screenshot and source code are parsed out as well.

## Dependencies

- Active [urlscan.io](urlscan.io) API key

## Documentation

### Triggers

- PipeConfig

### Organization Variables

This playbook expects the following organization variables:

- **keychain:** `urlscan.io API Key`
