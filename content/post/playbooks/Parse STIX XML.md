+++
date = "2018-09-04"
title = "Parse STIX XML"
tags = ["Parsing", "STIX", "XML"]
author = "joereese"
description = "Parse a STIX XML file from the File Post spaces app."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/parse-stix-xml"
downloadLinks = ["/post/playbooks/downloads/Parse STIX XML from File Post.pbx"]
+++

This playbook is intended to parse a STIX XML file from the File Post spaces app.  See [https://kb.threatconnect.com/customer/portal/articles/2920045](https://kb.threatconnect.com/customer/portal/articles/2920045) for how to configure and use the File Post app.

Once the playbook receives a file from the File Post app it will run the file through the STIX Parser playbook app and then import the data in ThreatConnect with the ThreatConnect Import app.  Additionally, it can save the uploaded file as a Document and associate the file to the indicators and groups that were created.  Results are returned to the user in the HTTP response.

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **body:** used in the "STIX 1.1.1 Parser 1" app
- **header:** used in the "Parse HTTP Header 1" app
- **body:** used in the "Create ThreatConnect Document 1" app
