+++
date = "2018-04-16"
title = "URL Text Reader"
tags = ["HTML", "URL"]
author = "Floyd Hightower"
description = "Request the content of the given website and return the text of the website's content."
categories = ["Playbooks"]
+++

This playbook is triggered with an HTTP Trigger which expects a URL to be POSTed to it. When a URL is POSTed, it will make a request to the URL and return the text from the URL's HTML.
