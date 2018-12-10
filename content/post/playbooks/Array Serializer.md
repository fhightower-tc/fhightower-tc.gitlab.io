+++
date = "2018-06-06"
title = "Array Iterator"
tags = ["Utility"]
author = "Floyd Hightower"
description = "Given an array, this playbook sends each item in the array one at a time to another playbook. This allows you to run a playbook on each item of an array."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/array-serializer"
downloadLinks = ["/post/playbooks/downloads/Array Serializer.pbx"]
+++

**YOU SHOULD STOP USING THIS PLAYBOOK. Instead, use the array iterator app described at [https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_Array_Iterator](https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_Array_Iterator).** If you cannot install custom apps, you should use the array iterator component here: [https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/array-iterator](https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/array-iterator).

## Usage

This playbook expects an array to be sent (as a string) in the body of an http POST request to the trigger of this playbook. It also requires a `link` query parameter providing the playbook trigger link to which you would like to send each item in the array. Each item in the array will be send to the playbook trigger link in the body of a request. A request to this app will look something like:

![Setup](images/array_serializer_setup.png)

To send data into this playbook, you must wrap the incoming data in square brackets ("[" and "]"). For example, let's say you have a string array. In order to send the data from this array into the array serializer, you would have to first pass the string array through the "Join Array" app to convert the array to a string. Next, in the "HTTP Client" app that calls the array serializer, the body should look something like:

```
[#joinedArray]
```

The joined array (which is a string), must be surrounded by square brackets.

## Use Cases

* Perform an action on each item in an array

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **body:** used in the "Json Path 1" app
- **body:** used in the "Find and Replace 1" app
- **queryparam:** used in the "Value Lookup 1" app
- **body:** used in the "Logger 1" app

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **triggerForThisPlaybook:** `https://sandbox.threatconnect.com/api/playbook/402b2179-b9a1-4085-9e6b-2604fb015b3d`
- **errorMessage:** `Request to #App:14487:link!String failed: #App:14488:http.status_code!String . Make sure this link is correct and that the playbook related to this link is turned on.`
- **errorMessage:** `Request to #App:14482:triggerForThisPlaybook!String failed: #App:14486:http.status_code!String . Make sure this link is correct (it should be the trigger link for this playbook).`
