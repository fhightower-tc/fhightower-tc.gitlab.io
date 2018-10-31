+++
date = "2018-03-07"
title = "Adjust DNS"
tags = ["DNS", "Indicators", "Hosts"]
author = "Floyd Hightower"
description = "These playbooks allow users to turn the DNS on or off for all indicators associated with a group."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/toggle-dns"
downloadLinks = ["/post/playbooks/downloads/Adjust DNS.pbx"]
+++

## Usage

Install all three of these playbooks and then install the array serializer playbook. Then edit the "Set Variable 1" app near the beginning of both the "Turn DNS Off Trigger" and "Turn DNS On Trigger" playbooks; you will need to provide the trigger link to the array serializer and the processing playbook (which is the "Adjust DNS" playbook in this case).

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **body:** used in the "ThreatConnect API 1" app
- **queryparam:** used in the "Value Lookup 1" app
