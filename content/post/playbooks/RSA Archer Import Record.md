+++
date = "2018-09-18"
title = "RSA Archer: Import Archer Record"
tags = ["RSA", "RSA Archer", "Importer", "Workflow", "Incidents"]
author = "joereese"
description = "Download and parse an RSA Archer record into a ThreatConnect incident."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/rsa-archer-import-record"
+++

This playbook starts with an HTTP Trigger which is intended to be triggered by an Archer advanced workflow.  Once triggered, the playbook will download and parse the Archer record based with the ID that was passed to it.  From there it will create a ThreatConnect Incident and save the  parsed fields in the Incident.  Additionally, it will parse the Actor saved on the Archer record and either save or associated it to the Incident in ThreatConnect.  Lastly, the Archer record is updated with the link back to the Incident in ThreatConnect.

## Documentation

### Triggers

- HttpLink

### HTTP Link Trigger

This playbook uses an HTTP trigger; the parts of the HTTP request below are used by the following apps:

- **queryparam:** used in the "Value Lookup" app

### Organization Variables

This playbook expects the following organization variables:

- **text:** `RSA Archer Username`
- **text:** `RSA Archer Instance Name`
- **keychain:** `RSA Archer Password`
- **text:** `RSA Archer Base URL`

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **v.attribute.aac:** 

```
**Threat Categories:** #App:21279:j.archer.json.threat_categories!String 
**Threat Vectors:** #App:21279:j.archer.json.threat_vectors!String 
**Threat Asset Types:** #App:21279:j.archer.json.target_asset_types!String 
**Threat Valid:** #App:21279:j.archer.json.threat_valid!String 
**Threat Actor:** #App:21279:j.archer.json.threat_actor!String
```

- **actor.doesnt_exist:** `No Actor in Archer Record`
- **actor.new:** `Actor #App:21285:tc.adversary.name!String was created in TheatConnect and associated with Incident`
- **actor.associated:** `Actor #App:21279:j.archer.json.threat_actor!String already exists in ThreatConnect and has been associated to the Incident`
