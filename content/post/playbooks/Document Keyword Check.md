+++
date = "2018-06-28"
title = "Key-word Parsing"
tags = ["Document", "Parsing"]
author = "billdauterive"
description = "These playbooks will allow you to define a set of keywords in a JSON Array to parse a document for. Upon ingestion of a document the playbook will parse the documents in the specified owners for the given keywords. Should a match be found the group name as well as the identified keywords will be added as tags on the triggering document."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/KeyWord%20Parsing"
+++

## Usage

Populate DataStore with Keywords - This Playbook will only need to be ran once, it will create an list of keywords in JSON format and submit them to a datastore in ElasticSearch for your Org called "keywords". The keywords themselves are stored in variables so they can be updated for easy of future additions.

Bearing in mind if you create a new array in the datastore the playbook "Keyword Check Playbook" would need to be updated to also parse for the new array.

Verify DataStore Data - will only need to be ran to verify the first playbook created the data that is expected.

Document Keyword Check - this is the actual playbook that does the work. Currently it is set to fire off the tag "parseme" to keep it from firing all of the time for performance implications, you can remove the tag requirement and it will fire off any and all documents created within the owner(s) specified for the document trigger.

When triggered, this will - Get the list of keywords from the datastore in ElasticSearch, JSON parse this list for the type and save them as variables Convert the document to a set of strings Do a regex capture on any keywords that match between the two For those that match it will create the tag for the group, ie: China/Russia It will additionally tag the document with the actual keywords within those that match, ie: APT12/APT28 etc.

## Documentation for "Document Keyword Check" Playbook

### Triggers

- Document

### Datastores

This playbook uses the following datastores:

- `GET organization/keywords/`:
  - **Datastore Organization:** "Customer Org"
  - **Datastore Entity:** ```{
          from: 0,
          size: 5000
        }```

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **enclosure.North_Korea:** `(#App:567:join.North_Korea!String)`
- **enclosure.China:** `(#App:567:join.China!String)`
- **enclosure.Russia:** `(#App:567:join.Russia!String)`

## Documentation for "Populate DataStore with Keywords" Playbook

### Triggers

- HttpLink

### Datastores

This playbook uses the following datastores:

- `POST organization/keywords/None`:
  - **Datastore Organization:** "Customer Org"
  - **Datastore Entity:** ```#App:623:North_Korea!String```

- `POST organization/keywords/None`:
  - **Datastore Organization:** "Customer Org"
  - **Datastore Entity:** ```#App:623:China!String```

- `POST organization/keywords/None`:
  - **Datastore Organization:** "Customer Org"
  - **Datastore Entity:** ```#App:623:Russia!String```

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **North_Korea:** `{    "data": [        {            "North_Korea": [                "APT37"            ]        }    ]}`
- **Russia:** `{    "data": [        {            "Russia": [                "APT29",                "APT28"            ]        }    ]}`
- **China:** `{    "data": [        {            "China": [                "APT30",                "APT27",                "APT19",                "APT18",                "APT17",                "APT16",                "APT12",                "APT10",                "APT3",                "APT1"            ]        }    ]}`

## Documentation for "Verify DataStore Data" Playbook

### Triggers

- HttpLink

### Datastores

This playbook uses the following datastores:

- `GET organization/keywords/`:
  - **Datastore Organization:** "Customer Org"
  - **Datastore Entity:** ```{from: 0,size: 5000}```
