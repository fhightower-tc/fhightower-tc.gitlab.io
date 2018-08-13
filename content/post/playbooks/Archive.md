+++
date = "2018-03-08"
title = "Archive.org Wayback Machine Query"
tags = ["Archive.org", "Hosts", "URLs", "Enrichment"]
author = "Floyd Hightower"
description = "Query for a Host or URL Indicator in <a href='https://archive.org/web/web.php'>Archive.org's Wayback Machine</a>."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/archive-org-wayback-machine-query"
+++

## Documentation

### Triggers

- UserAction

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **successMessage:** `This indicator was archived on #App:12676:archiveDate!String . You can view it here:<a href="#App:12676:archiveURL!String " target="_blank"> #App:12676:archiveURL!String</a>.`
- **failureMessage:** `This indicator was not found in archive.org.`
