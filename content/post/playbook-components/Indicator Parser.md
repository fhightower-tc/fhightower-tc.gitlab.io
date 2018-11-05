+++
date = "2018-02-28"
title = "Indicator Parser"
tags = ["Indicators", "Parsing"]
author = "Floyd Hightower"
description = "Parse indicators from text using the system regexes available via the API."
categories = ["Playbook Components"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/indicator-parser"
downloadLinks = ["/post/playbook-components/downloads/Indicator Parser.pbx"]
+++

The API endpoint to get the system regexes is documented [here](https://docs.threatconnect.com/en/latest/rest_api/indicators/indicators.html#retrieve-available-indicator-types).

## Dependencies

- [Deduplicator app](https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_Deduplicator)

## Documentation

### Triggers

- PipeConfig

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **addressRegexUrl:** `/v2/types/indicatorTypes/Address`
- **emailAddressRegexUrl:** `/v2/types/indicatorTypes/EmailAddress`
- **fileRegexUrl:** `/v2/types/indicatorTypes/File`
- **hostRegexUrl:** `/v2/types/indicatorTypes/Host`
- **urlRegexUrl:** `/v2/types/indicatorTypes/Url`
- **errorMessagePrefix:** `[Indicator Parser PB]:`
