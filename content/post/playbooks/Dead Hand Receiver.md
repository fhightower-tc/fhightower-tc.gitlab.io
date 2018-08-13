+++
date = "2018-06-19"
title = "Dead Hand Receiver"
tags = ["Dead Hand", "Utility"]
author = "Malware Utkonos"
description = "This playbook receives a webhook from a feed collector and then resets the dead hand entry in the datastore. This prevents the dead hand timer from sending a fault notification. This playbook also checks for indicator and group counts and sends an appropriate notification if groups or indicators are not collected."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/Dead%20Hand"
+++

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **queryparam:** used in the "Lookup Counts" app

### Organization Variables

This playbook expects the following organization variables:

- **keychain:** `Slack Token`

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **datastore_path:** `collect_abusech_feodo_ip`
- **base_message:** `Collect: abuse.ch Feodo IP`
- **slack_channel:** `innovation`
