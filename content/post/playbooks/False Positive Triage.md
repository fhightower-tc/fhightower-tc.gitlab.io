+++
date = "2018-06-20"
title = "False Positive Triage"
tags = ["False Positives", "Indicators", "Cleaning"]
author = "Malware Utkonos"
description = "Reports a false positive, turns off all monitors, resets all ratings, waits 25 hours for CAL to pick up the change, and finally deletes the indicator and republishes all groups associated with the indicator."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/False%20Positive%20Triage"
downloadLinks = ["/post/playbooks/downloads/False Positive Triage HTTP Interface.pbx", "/post/playbooks/downloads/False Positive Triage Trigger Interface.pbx", "/post/playbooks/downloads/False Positive Triage Standalone - pre 5.7.pbx", "/post/playbooks/downloads/False Positive Triage Standalone - post 5.7.pbx"]
+++

There are two versions of this playbook. One which works in ThreatConnect instances before version 5.7 and one that works in versions >= 5.7.

## Pre 5.7 Version

This playbook triages false positives by:

- reporting a false positive
- turning off all monitors (DNS/WHOIS)
- resetting all ratings

Everything in the [pre-5.7 directory](https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/False%20Positive%20Triage/pre-5.7) will work in ThreatConnect versions before 5.7. The `pre-5.7/False Positive Triage Standalone - pre 5.7.pbx` playbook can be installed on its own and provides a user-action trigger to triage false positives. There are also two interfaces (`pre-5.7/False Positive Triage HTTP Interface.pbx` and `pre-5.7/False Positive Triage Trigger Interface.pbx`) which provide different interfaces with the false positive triage component [here](https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/components/false-positive-triage). The advantage of this structure (as described [here](https://pb-constructs.hightower.space/playbooks/paradigms/structuring-playbook-systems)) is that it is more flexible and interface-agnostic.

### Documentation

#### Triggers

- UserAction

#### Datastores

This playbook uses the following datastores:

- `POST organization/falsePositives/None`:
  - **Datastore Organization:** <NO ORGANIZATION SPECIFIED>
  - **Datastore Entity:** ```#App:1445141972:tc.indicator!TCEntity```

## Post 5.7 Version

This playbook triages false positives by:

- reporting a false positive
- turning off all monitors (DNS/WHOIS)
- resetting all ratings
- waiting for 25 hours (to make sure CAL gets the new information)
- deleting the indicator
- republishing all groups previously associated with the indicator

Everything in the [post-5.7 directory](https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/False%20Positive%20Triage/post-5.7) will only work in ThreatConnect versions after the release of version 5.7.

### Documentation

#### Triggers

- UserAction
