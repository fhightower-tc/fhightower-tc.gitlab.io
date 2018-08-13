+++
date = "2018-06-19"
title = "Dead Hand Timer"
tags = ["Dead Hand"]
author = "Malware Utkonos"
description = "This playbook checks the status of a feed and sends a notification if there is a fault in the feed status."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/Dead%20Hand"
+++

## Documentation

### Triggers

- Timer

### Organization Variables

This playbook expects the following organization variables:

- **keychain:** `Slack Token`

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **datastore_path:** `collect_abusech_feodo_ip`
- **message:** `Feed Failure: Collect: abuse.ch Feodo IP`
- **slack_channel:** `innovation`
