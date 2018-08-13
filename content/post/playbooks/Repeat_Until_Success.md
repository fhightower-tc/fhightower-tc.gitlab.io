+++
date = "2018-04-30"
title = "Repeat Until Successful"
tags = ["Utility"]
author = "Floyd Hightower"
description = "This playbook attempts an action until it is successful. In this sense, it is a bit like a 'pause' or 'wait' command that will wait until the given action is successful before moving on."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/repeat-until-success"
+++

## Usage

This playbook is triggered by an HTTP request with the following query parameters:

- `count`: The number of times the action has been attempted (when triggering this playbook, you will usually want to set this value to zero)
- `link`: The http trigger link to the playbook with the action you would like to perform
- `max`: The maximum number of times to attempt the action

The basic algorithm is as follows:

1. Attempt an http request to the playbook specified by the `link` URL query parameter.
2. If the http request from step 1 works: we're done!
3. If the http request from step 1 does not work (returns 40X error):
    - Increment the count which keeps track of the number of times we have tried to trigger the other playbook
    - If the count is less than the maximum number of attempts: wait for twenty seconds and make another attempt
    - If the count is equal to the maximum number of attempts: stop and send a message (by default, a slack message)

## Use Cases

* Wait until a condition is true before proceeding
* Attempt an action until the action is successful

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **body:** used in the "http - attempt action" app
- **queryparam:** used in the "Value Lookup 1" app
- **body:** used in the "http - call this playbook again" app

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **messagePrefix:** `[repeat until complete]:`
- **thisPlaybookTrigger:** `REPLACE ME!`
- **newCount:** `#App:17375:http.content!String`
