+++
date = "2018-04-16"
title = "PDF Reader"
tags = ["PDF", "Parsing"]
author = "Floyd Hightower"
description = "Request a PDF from a given URL and return the text from the PDF."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/pdf-reader"
downloadLinks = ["/post/playbooks/downloads/PDF_reader.pbx"]
+++

## Usage

This playbook is triggered with an HTTP Trigger which expects a URL (which is a link to a PDF) to be posted to it. When a link is posted to it, it will request the content of the PDF and return its text contents.

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **body:** used in the "HTTP Client 2" app
