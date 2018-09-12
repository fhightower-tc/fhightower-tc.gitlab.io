+++
date = "2018-06-20"
title = "False Positive Triage"
tags = ["False Positives", "Indicators", "Cleaning"]
author = "Malware Utkonos"
description = "Reports a false positive, turns off all monitors, resets all ratings, waits 25 hours for CAL to pick up the change, and finally deletes the indicator and republishes all groups associated with the indicator."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/False%20Positive%20Triage"
+++

There are two versions of this playbook. One which works in ThreatConnect instances before version 5.7 and one that works in versions after 5.7.

## Documentation

### Pre 5.7 Version

Rather than deleting the indicator and republishing associated groups after 25 hours, this playbook writes the indicator data into the datastore so it can be triaged using a script or other mechanism.

#### Triggers

- UserAction

#### Datastores

This playbook uses the following datastores:

- `POST organization/falsePositives/None`:
  - **Datastore Organization:** <NO ORGANIZATION SPECIFIED>
  - **Datastore Entity:** ```#App:1445141972:tc.indicator!TCEntity```

### Post 5.7 Version

#### Triggers

- UserAction
