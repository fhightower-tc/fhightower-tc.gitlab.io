+++
date = "2018-05-14"
title = "Page Monitor"
tags = ["Monitoring", "Website"]
author = "Floyd Hightower"
description = "Periodically capture the content of a website and send an alert if the content changes."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/page-monitor-playbook"
downloadLinks = ["/post/playbooks/downloads/Page Monitor < 5.6.pbx", "/post/playbooks/downloads/Page Monitor.pbx"]
+++

**Warning:** Do **NOT** use this playbook to monitor malicious websites. It is only designed to monitor benign infrastructure.

## Dependencies

- The "Page Monitor.pbx" playbook will work in any ThreatConnect instance where the version is >= 5.6
- The "Page Monitor < 5.6.pbx" playbook will work in any ThreatConnect instance where the version is < 5.6

## Documentation

### Triggers

- Timer

### Datastores

This playbook uses the following datastores:

- `GET local/pageMonitor/`:
  - **Datastore Organization:** <NO ORGANIZATION SPECIFIED>
  

- `POST local/pageMonitor/#App:10146:databaseID!String`:
  - **Datastore Organization:** <NO ORGANIZATION SPECIFIED>
  - **Datastore Entity:** ```{"hash": "#App:10129:hash.encode.md5!String"}```

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **userAgent:** `Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/53.0.2785.143 Safari/537.36`
- **slackChannel:** <NO VALUE GIVEN>
- **website:** `http://example.com`
- **slackMessagePrefix:** `[Page Monitor PB]`
- **nonExistHash:** `0`
