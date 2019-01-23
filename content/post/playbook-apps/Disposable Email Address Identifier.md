+++
date = "2018-12-23"
title = "Disposable Email Addresses"
tags = ["Disposable Email Addresses", "Enrichment", "Email Addresses"]
author = "Floyd Hightower"
description = "Determine if an email address is disposable or not using the domain name of the email address."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_Disposable_Email_Address_Identifier"
+++

# Disposable Email Address Identifier

Determine if the domain name of an email address is a disposable email address or not (using the list available here: [https://raw.githubusercontent.com/martenson/disposable-email-domains/master/disposable_email_blocklist.conf](https://raw.githubusercontent.com/martenson/disposable-email-domains/master/disposable_email_blocklist.conf)).

## Inputs

This playbook app takes either an email address or host as input.

## Outputs

This playbook returns a `0` (zero) if the email address's hostname (or the hostname if just given a hostname) is NOT a disposable email address service and `1` if the hostname is a disposable email address service.

## Examples

- `example@mailinator.com` => `1`
- `example@example.com` => `0`
