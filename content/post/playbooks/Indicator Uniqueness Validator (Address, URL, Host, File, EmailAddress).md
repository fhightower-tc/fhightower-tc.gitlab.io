+++
date = "2018-06-08"
title = "Indicator Uniqueness Validator"
tags = ["Indicators"]
author = "citadelintellgenceresearch"
description = "This playbook is designed to verify when a new IOC (Address, URL, Host, File, or Email Address) comes in, whether it already exists in the platform in a different owner."
categories = ["Playbooks"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/playbooks/indicator%20uniqueness%20validator"
downloadLinks = ["/post/playbooks/downloads/Indicator Uniqueness Validator (Address, URL, Host, File, EmailAddress).pbx"]
+++

This playbook is designed to verify when a new IOC (Address, URL, Host, File, or Email Address) comes in, whether it already exists in the platform in a different owner. If so, the new indicator is tagged with "multiple_owners", denoting that it is a duplicate IOC. This is designed to be used in conjunction with a custom dashboard card to display the owner names and their number of duplicate indicators. The TQL syntax for the dashboard card is as follows:

```
typeName in ("Address", "EmailAddress", "File", "Host", "URL") and tag in ("multiple_owners")
```

For the card, choose to display as a chart and group by Owner Name. For chart type, ideally, you'd choose between either a Number Card if all you want to see is the total number of duplicate IOCs per source, or an Advanced Pie Chart if you'd to see the total number of duplicate IOCs in your instance, with that number broken down per source with a percentage as well.

**NOTE:** This is designed to run on every single IOC that gets added in the owners that you choose in the trigger. This can mean quite a lot of times this Playbook runs. For that reason, I've restricted it to the 5 main IOC types. If you wish to open this functionality up to other IOC types, please contact me at jlakeson@citadelintelligenceresearch.com

## Documentation

### Triggers

- MultipleIndicator
