+++
date = "2018-03-05"
title = "Indicator Comment Link Creator"
tags = ["Sharing", "Indicators", "Comments", "Links"]
author = "Floyd Hightower"
description = "Create and copy the link to an Indicator in two clicks."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/comment-link-creators"
downloadLinks = ["/post/playbooks/downloads/indicator comment link creator.pbx"]
+++

This playbook was featured in a "Playbook Friday" blog: [https://threatconnect.com/blog/playbook-fridays-group-and-indicator-comment-link-creators/](https://threatconnect.com/blog/playbook-fridays-group-and-indicator-comment-link-creators/)! The blog post includes installation instructions for this playbook.

![](/post/playbooks/images/indicator-comment-link-creator.png)

## Documentation

### Triggers

- UserAction

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **errorMessagePrefix:** `[Indictor Comment Link Creator PB]:`
- **shareCommentLink:** `[[#Trigger:1066:trg.action.type!String:#Trigger:1066:trg.action.item!String]]`
