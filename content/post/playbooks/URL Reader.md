+++
date = "2018-04-16"
title = "URL Reader"
tags = ["HTML", "Parsing"]
author = "Floyd Hightower"
description = "Request the content of the given website and return the text of the website's content."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/url-reader"
downloadLinks = ["/post/playbooks/downloads/URL_reader.pbx"]
+++

## Dependencies

- [HTML Text Parser](https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_HTML_Text_Parser)

## Usage

This playbook is triggered with an HTTP Trigger which expects a URL to be POSTed to it. When a URL is POSTed, it will make a request to the URL and return the text from the URL's HTML.

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **body:** used in the "HTTP Client 2" app
