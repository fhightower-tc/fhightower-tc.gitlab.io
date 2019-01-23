+++
date = "2019-01-18"
title = "CSV to JSON"
tags = ["CSV", "JSON", "Converting Data", "Structured Data"]
author = "Floyd Hightower"
description = "Convert CSV to JSON."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_CSV_to_JSON"
+++

# CSV to JSON

This app converts CSV to JSON using Floyd Hightower's [CSV to JSON](https://gitlab.com/fhightower/csv-to-json) package.

For example, this:

```
foo,bar
1,2
```

Becomes this:

```
[{'a': 'foo', 'b': 'bar'}, {'a': '1', 'b': '2'}]
```

Or you can specify a row of the CSV to be used as the keys for the CSV. For example, the output below shows what happens when the `heading_row` is set to zero:

```
[{'foo': '1', 'bar': '2'}]
```

## Release Notes

### 0.1.0

* Initial Release
