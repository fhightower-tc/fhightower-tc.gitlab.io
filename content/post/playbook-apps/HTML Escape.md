+++
date = "2019-01-04"
title = "HTML Escape"
tags = ["HTML", "Converting Data"]
author = "Floyd Hightower"
description = "Escape html."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_HTML_Escape"
+++

# HTML Escape

This app escapes html such as:

- `crime & punishment` => `crime &amp; punishment`
- `<p>Atlas ¯\_(ツ)_/¯'ed</p>` => `&lt;p&gt;Atlas ¯\\_(ツ)_/¯&#x27;ed&lt;/p&gt;`
- `<s>Paradise</s>` => `&lt;s&gt;Paradise&lt;/s&gt;`

## Release Notes

### 0.0.1

* Initial Release
