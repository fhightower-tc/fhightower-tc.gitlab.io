+++
date = "2018-03-10"
title = "JSON Builder"
tags = ["JSON"]
author = "Bracey Summers"
description = "Take a JSON formatted String with embedded variables and output a JSON String."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_JSON_Builder"
+++

# Release Notes
## 1.0.0
* Initial Release

---

# Summary
This playbook App will take a JSON formatted String with embedded variables and output a JSON String.

> Note: String value must be wrapped in double quotes.  All other values should **not** have double quotes.

![Inputs](/post/playbook-apps/images/info-json-builder.png)

# Dependencies
* tcex>=0.7,<0.8

# Input Definitions
* JSON Data - The JSON string to resolve embedded variables.

![Inputs](/post/playbook-apps/images/inputs-json-builder.png)

# Output Definitions
* json.data - The JSON String with optional embedded variables resolved.

![Inputs](/post/playbook-apps/images/outputs-json-builder.png)

# Building

```
pip install tcex
tclib
tcpackage
```

# Local Testing

All the environment variables in `tcex.d/profiles/json_builder.json` file must be set on the local system.

```
tcrun --group qa-build
```
