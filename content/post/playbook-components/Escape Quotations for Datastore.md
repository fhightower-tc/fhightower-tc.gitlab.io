+++
date = "2018-06-14"
title = "Escape Quotes for Datastore"
tags = ["Datastore", "Cleaning"]
author = "Floyd Hightower"
description = "Escape quotation marks for storing content in the datastore."
categories = ["Playbook Components"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/escape-quotation-marks-for-datastore"
+++

If you're trying to store an object or array in the [datastore](https://pb-constructs.hightower.space/playbooks/introductions/datastore) as a string, you will first need to escape all of the quotations in the object/array. This component is designed to do that.

## Input

As input, this component requires a string in which all double quotation marks (`"`) will be escaped.

## Output

This component returns the input item with quotation marks escaped for storage in the datastore.

## Documentation

### Triggers

- PipeConfig
