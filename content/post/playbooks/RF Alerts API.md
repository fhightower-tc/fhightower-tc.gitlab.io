+++
date = "2018-03-16"
title = "Recorded Future Alerts API"
tags = ["Recorded Future"]
author = "brikardtc"
description = "These 2 Playbooks will query the Recorded Future API for any alerts for the specified timed period from the \"Timer\" in the RF Alerts Query Playbook. The secondary Playbook (RF Incident Create) will then create incidents from the Recorded Future API."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/Recorded%20Future%20Alerts%20API"
downloadLinks = ["/post/playbooks/downloads/RF Alerts Incident Create.pbx", "/post/playbooks/downloads/RF Alerts Query.pbx"]
+++

## Documentation for "RF Alerts Incident Create" Playbook

### Triggers

- CVE
- Task

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **RF:** `Recorded Future Alert`
- **XRFToken:** `your_api_key_here`

## Documentation for "RF Alerts Query" Playbook

### Triggers

- Timer

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **XRFToken:** `your_API_TOKEN_HERE`
