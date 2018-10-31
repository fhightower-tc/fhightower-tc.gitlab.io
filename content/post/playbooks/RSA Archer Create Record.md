+++
date = "2018-09-18"
title = "RSA Archer: Create Archer Record"
tags = ["RSA", "RSA Archer", "Importer", "Workflow", "Incidents"]
author = "joereese"
description = "Create an RSA Archer record from an incident in ThreatConnect"
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/rsa-archer-create-record"
downloadLinks = ["/post/playbooks/downloads/RSA Archer _ Create Archer Record from Incident.pbx"]
+++

This playbook starts with a User Action trigger tied to ThreatConnect Incidents.  When triggered it will parse the Incident attributes and create an Archer record with relevant fields.

## Documentation

### Triggers

- UserAction

### Organization Variables

This playbook expects the following organization variables:

- **keychain:** `RSA Archer Password`
- **text:** `RSA Archer Username`
- **text:** `RSA Archer Instance Name`
- **text:** `RSA Archer Base URL`
