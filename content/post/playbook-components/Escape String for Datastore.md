+++
date = "2018-06-14"
title = "Escape Strings for Datastore"
tags = ["Datastore", "Cleaning"]
author = "Floyd Hightower"
description = "Escape strings for the datastore."
categories = ["Playbook Components"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/escape-string-for-datastore"
downloadLinks = ["/post/playbook-components/downloads/[utility] Escape String for Datastore.pbx"]
+++

If you're trying to store an object or array in the [datastore](https://pb-constructs.hightower.space/playbooks/introductions/datastore) as a string, you will first need to escape all of the quotations in the object/array. This component is designed to do that.

## Input

As input, this component requires a string.

## Output

This component returns the input item with quotation marks and newlines escaped for storage in the datastore.

## Documentation

### Triggers

- PipeConfig
