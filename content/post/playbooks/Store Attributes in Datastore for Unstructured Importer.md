+++
date = "2018-10-10"
title = "Store Attributes in Datastore for Unstructured Indicator Importer"
tags = ["Indicators", "Importer", "Attributes", "Datastore", "Unstructured Data"]
author = "Floyd Hightower"
description = "Store attributes for the unstructured indicator importer in the datastore."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/unstructured-data-importer-attribute-storer"
+++

This playbook stores attributes from [https://gitlab.com/fhightower-tc/unstructured-indicator-importer/blob/master/example_datastore_attributes.json](https://gitlab.com/fhightower-tc/unstructured-indicator-importer/blob/master/example_datastore_attributes.json) in the datastore so that they can be accessed by the [unstructured indicator importer](https://gitlab.com/fhightower-tc/unstructured-indicator-importer).

For more details, please see [https://gitlab.com/fhightower-tc/unstructured-indicator-importer#attributes-in-datastore-required](https://gitlab.com/fhightower-tc/unstructured-indicator-importer#attributes-in-datastore-required).

## Documentation

### Triggers

- HttpLink

### Datastores

This playbook uses the following datastores:

- `POST organization/app-data/attributeTest`:
  - **Datastore Organization:** <NO ORGANIZATION SPECIFIED>
  - **Datastore Entity:** ```{"text": "#App:22601:escapedString!String"}```

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **attributeJsonUrl:** `https://gitlab.com/fhightower-tc/unstructured-indicator-importer/raw/master/example_datastore_attributes.json`
