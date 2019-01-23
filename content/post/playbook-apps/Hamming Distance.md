+++
date = "2019-01-18"
title = "Hamming Distance"
tags = ["Hamming Distance", "Strings"]
author = "Floyd Hightower"
description = "Find the <a href="https://en.wikipedia.org/wiki/Hamming_distance">hamming distance</a> between two strings."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_Hamming_Distance"
+++

# Hamming Distance

Playbook app to find the [Hamming Distance]() (the number of positions at which the corresponding symbols are different) between two strings.

For example, given `abc` and `abd`, the hamming distance is 1 (only the last letter is different). Given `abc` and `cbd`, the hamming distance is 2 (The first and last letters of the two strings are different).

# Usage

## Inputs

This playbook has two, required inputs:

- `string_1` (required): a string whose length you would like to compare with `string_2`
- `string_2` (required): a string whose length you would like to compare with `string_1`

Both `string_1` and `string_2` must be **the same length**.

## Outputs

The app outputs two variables:

- `hammingDistance`: The hamming distance (e.g. )
- `hammingDistance.percentage`: The hamming distance as a percentage of the length of the input strings (e.g. )

## Release Notes

### 0.1.0

* Initial Release
