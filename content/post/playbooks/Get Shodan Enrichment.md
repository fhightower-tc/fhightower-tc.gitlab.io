+++
date = "2018-03-21"
title = "Get Shodan Enrichment"
tags = ["Shodan", "Enrichment", "Indicators"]
author = "citadelintelligenceresearch"
description = "This playbook presents a User Action trigger that when pressed, will query Shodan's API for a given indicator then pull back enrichments and store them as an attribute on said indicator."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/Get%20Shodan%20Enrichment"
downloadLinks = ["/post/playbooks/downloads/Get Shodan Enrichment.pbx"]
+++

## Documentation

### Triggers

- PipeConfig

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **os.failure:** `OS Not Found`
- **os.success:** `#App:16217:json_path.output!String`
