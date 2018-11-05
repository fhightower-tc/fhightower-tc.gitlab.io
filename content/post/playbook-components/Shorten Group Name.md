+++
date = "2018-04-06"
title = "Shorten Group Name"
tags = ["Groups", "Names", "Utility"]
author = "Floyd Hightower"
description = "Shorten a group's name to the maximum length (100 characters)."
categories = ["Playbook Components"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/shorten_group_name"
downloadLinks = ["/post/playbook-components/downloads/Shorten Group Name.pbx"]
+++

This component takes a potential group name, shortens it to under the 100 character limit without splitting up any words in the group name, and adds a `...` at the end of it.

## Documentation

### Triggers

- PipeConfig

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **newGroupName:** `#App:16076:find_replace.output!String...`
- **originalGroupName:** `#App:16076:find_replace.output!String`
