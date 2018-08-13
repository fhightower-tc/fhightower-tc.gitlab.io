+++
date = "2018-06-06"
title = "Bro Intel Framework Signature Generator"
tags = ["BIF", "Bro", "Signatures", "Indicators"]
author = "Malware Utkonos"
description = "Generate a Bro Intelligence Framework signature from an indicator."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/BIF%20Signature%20Generator"
+++

## Documentation

### Triggers

- UserAction

### Variables Declared in the Playbook

The following variables are declared in this playbook:

- **bro.sig:** `#App:18829:merged.indicator!String	#App:18829:merged.bif_type!String	ThreatConnect	#App:18834:tc.indicator.description!String	#Trigger:1887:trg.action.weblink!String`
- **bro.sig:** `#App:18829:merged.indicator!String	#App:18829:merged.bif_type!String	ThreatConnect	No Description	#Trigger:1887:trg.action.weblink!String`
- **bif_type:** `Intel::ADDR`
- **indicator:** `#Trigger:1887:trg.action.item!String`
- **bif_type:** `Intel::DOMAIN`
- **indicator:** `#Trigger:1887:trg.action.item!String`
- **bif_type:** `Intel::EMAIL`
- **indicator:** `#Trigger:1887:trg.action.item!String`
- **bif_type:** `Intel::URL`
- **bif_type:** `Intel::SUBNET`
- **indicator:** `#Trigger:1887:trg.action.item!String`
- **bif_type:** `Intel::FILE_HASH`
- **indicator:** `#App:18843:tc.file.sha256!String`
- **indicator:** `#App:18843:tc.file.sha1!String`
- **indicator:** `#App:18843:tc.file.md5!String`
- **raw_data:** `BIF: #App:18829:merged.indicator!String`
