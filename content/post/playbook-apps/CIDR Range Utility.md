+++
date = "2019-01-04"
title = "CIDR Range Utility"
tags = ["CIDR", "Utility", "Indicators", "Broadcast Address", "Hostmak", "Netmask"]
author = "Floyd Hightower"
description = "Perform operations and get data from a CIDR range."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_CIDR_Range_Utility"
+++

# CIDR Range Utility

This app allows you to perform the following operations on CIDR range indicators:

- Get the number of IP Addresses included in the range
- Get the range as a string (e.g. `8.8.8.0/24` => `8.8.8.0 - 8.8.8.255`)
- Get the [broadcast address](https://en.wikipedia.org/wiki/Broadcast_address) of the range
- Get the [hostmask](https://www.ipconvertertools.com/convert-cidr-manually-binary) of the range
- Get the [netmask](https://www.ipconvertertools.com/convert-cidr-manually-binary) of the range

## Release Notes

### 0.0.1

* Initial Release
