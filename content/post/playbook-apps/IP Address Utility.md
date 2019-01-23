+++
date = "2019-01-04"
title = "IP Address Utility"
tags = ["IPs", "Utility", "Indicators", "IPv4", "IPv6"]
author = "Floyd Hightower"
description = "Perform operations and get data from an IP address."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_IP_Address_Utility"
+++

# IP Address Utility

This app allows you to perform the following operations on IP Address indicators:

- Determine whether or not the IP Address is private
- Determine whether or not the IP Address is reserved
- Determine the version of the IP Address (`4` or `6`)

If the IP Address is ipv6, it will also:

- Expand/explode the address (e.g. `2001:db8::1000` => `2001:0db8:0000:0000:0000:0000:0000:1000`)
- Compress/collapse the address (`2001:0db8:0000:0000:0000:0000:0000:1000` => `2001:db8::1000`)
- Format the address into the form required by ThreatConnect; for example:
  - `2001:db8::1000` => `2001:db8:0:0:0:0:0:1000`
  - `2001:0db8:0000:0000:0000:0000:0000:1000` => `2001:db8:0:0:0:0:0:1000`

## Release Notes

### 0.0.1

* Initial Release
