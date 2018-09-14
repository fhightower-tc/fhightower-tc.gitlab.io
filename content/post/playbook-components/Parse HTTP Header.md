+++
date = "2018-09-01"
title = "Parse HTTP Header"
tags = ["Parsing", "HTTP"]
author = "joereese"
description = "Parse the header from the HTTP Trigger (#trg.http.header) into useful output variables."
categories = ["Playbook Components"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/parse-http-header"
+++

This component parses the HTTP Header KeyValueArray into output variables.  It can be used downstream from both the HTTP Trigger and the HTTP Client app.  It also grabs the filename from the Content-Disposition header if it exists.  

The following output variables are currently defined: 

- http.header.accept
- http.header.accept_encoding
- http.header.accept_language
- http.header.accept_version
- http.header.authorization
- http.header.connection
- http.header.content_disposition
- http.header.content_disposition.file_name
- http.header.content_length
- http.header.content_type
- http.header.cookie
- http.header.date
- http.header.host
- http.header.user_agent

## Documentation

### Triggers

- PipeConfig

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **v.filename:** ` `
