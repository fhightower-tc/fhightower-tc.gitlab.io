+++
date = "2018-03-07"
title = "Toggle DNS"
tags = ["DNS", "Hosts"]
author = "Floyd Hightower"
description = "Turn on or off the DNS for all indicators associated with a group."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/toggle-dns"
+++

It uses the process of collecting, serializing, and processing described [here](https://fhightower.gitbooks.io/threatconnect-playbook-paradigms-and-constructs/content/constructs/collect_serialize_process.html).

## Usage

Install all three of these playbooks and then install the array serializer playbook. Then edit the "Set Variable 1" app near the beginning of both the "Turn DNS Off Trigger" and "Turn DNS On Trigger" playbooks; you will need to provide the trigger link to the array serializer and the processing playbook (which is the "Adjust DNS" playbook in this case).

## Dependencies

- [Array Serializer Playbook](link)

## Documentation for "Turn DNS Off Trigger" Playbook

### Triggers

- UserAction

### User Variables

This playbook expects the following user variables:

- **text:** `Personal Slack Channel`
- **keychain:** `Slack API Token`

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **errorMessagePrefix:** `[Turn DNS Off PB]:`
- **arraySerializerUrl:** `<REPLACE ME>`
- **adjustDNSPbUrl:** `<REPLACE ME>`

## Documentation for "Turn DNS On Trigger" Playbook

### Triggers

* UserAction

### User Variables

This playbook expects the following user variables:

* **keychain:** `Slack API Token`
* **text:** `Personal Slack Channel`

### Variables Declared in the Playbook

The following variables are declared in this playbook:

* **errorMessagePrefix:** `[Turn DNS On PB]:`
* **arraySerializerUrl:** `<REPLACE ME>`
* **adjustDNSPbUrl:** `<REPLACE ME>`
