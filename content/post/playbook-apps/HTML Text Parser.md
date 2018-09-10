+++
date = "2018-03-07"
title = "HTML Text Parser"
tags = ["HTML", "Parsing"]
author = "Floyd Hightower"
description = "Parse text from html."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_HTML_Text_Parser"
+++

# Summary

Parse text from html.

# Dependencies

- tcex
- beautifulsoup4

# Input Definitions

- `HTML Input`: The html from which you would like to parse the text

# Output Definitions

- `html_parser.text`: The text from the given html

# Installing in ThreatConnect

To install this app in ThreatConnect, run:

```shell
make lib
make pack
```

This will create a `.tcx` file in the top app directory which will work in ThreatConnect assuming the instance of ThreatConnect is running the same version of python used during the `make lib` command.

# Credits

This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and [Floyd Hightower's TCEX App Template](https://gitlab.com/fhightower-templates/tcex-app-template).
