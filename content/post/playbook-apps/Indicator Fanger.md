+++
date = "2018-03-02"
title = "Indicator Fanger"
tags = ["Indicators", "Fanging"]
author = "Floyd Hightower"
description = "Fang indicators of compromise in text."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_Indicator_Fanger"
downloadLink = "/post/playbook-apps/downloads/TCPB_-_Indicator_Fanger_v0.1.tcx"
+++

# Summary

Fang indicators of compromise in text. Fanging the process of `example[.]com hXXp://bad[.]com/phishing.php` => `example.com http://bad.com/phishing.php` (see https://ioc-fang.github.io/ for more information on fanging and defanging indicators).

# Dependencies

- tcex
- [ioc_fanger](https://github.com/ioc-fang/ioc_fanger)

# Input Definitions

- `Text`: The text which you would like to fang

# Output Definitions

- `fangedText`: The text with indicators fanged

# Credits

This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and [Floyd Hightower's TCEX App Template](https://gitlab.com/fhightower-templates/tcex-app-template).
