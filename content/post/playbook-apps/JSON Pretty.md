+++
date = "2018-03-10"
title = "JSON Pretty"
tags = ["JSON"]
author = "Bracey Summers"
description = "Take a JSON String and format it for pretty output."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_JSON_Pretty"
+++

# Release Notes
## 1.0.0
* Initial Release

---

# Summary
This playbook App will take a JSON String and format it for pretty output.

![Info](/post/playbook-apps/images/info-json-pretty.png)

# Dependencies
* tcex>=0.7,<0.8

# Input Definitions
* JSON Data - The JSON string to be formatted.
* Indent - The number of spaces to indent each section.
* Sort Keys - Whether or not to sort keys.

![Inputs](/post/playbook-apps/images/inputs-json-pretty.png)

# Output Definitions
* json.pretty - The formatted JSON String.

![Outputs](/post/playbook-apps/images/outputs-json-pretty.png)

# Building

```
pip install tcex
tclib
tcpackage
```

# Local Testing

All the environment variables in `tcex.d/profiles/pretty.json` file must be set on the local system.

```
tcrun --group qa-build
```
