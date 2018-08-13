+++
date = "2018-03-08"
title = "Attribute and Tag Adder"
tags = ["Attributes", "Tags", "Indicators", "Metadata"]
author = "Floyd Hightower"
description = "Add an attribute and/or tag to all indicators associated with a given group."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/attribute-and-tag-adder"
+++

## Documentation

### Trigger Playbook

#### Triggers

- UserAction

#### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **groupID:** `#Trigger:1044:trg.action.item!String`
- **metadataAddingPlaybookTrigger:** <NO VALUE GIVEN>

### Attribute and Tag Adding Playbook

#### Triggers

- HttpLink

#### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **body:** used in the "Decode URL 1" app

#### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **errorMessagePrefix:** `[Attribute and Tag Adder PB]:`
