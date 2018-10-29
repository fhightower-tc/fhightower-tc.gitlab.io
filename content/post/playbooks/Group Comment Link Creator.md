+++
date = "2018-03-05"
title = "Group Comment Link Creator"
tags = ["Sharing", "Groups", "Comments", "Links"]
author = "Floyd Hightower"
description = "Create and copy the link to a Group in two clicks."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/comment-link-creators"
+++

This playbook was featured in a "Playbook Friday" blog: [https://threatconnect.com/blog/playbook-fridays-group-and-indicator-comment-link-creators/](https://threatconnect.com/blog/playbook-fridays-group-and-indicator-comment-link-creators/)! The blog post includes installation instructions and a gif of how to setup the playbook.

![](/post/playbooks/images/group-comment-link-creator.png)

## Documentation

### Triggers

- UserAction

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **errorMessagePrefix:** `[Group Comment Link Creator PB]:`
- **shareCommentLink:** `[[#Trigger:1067:trg.action.type!String:#App:11439:groupName!String]]`