+++
date = "2018-03-10"
title = "Array Set Operations"
tags = ["Arrays", "Lists", "Sets"]
author = "Bracey Summers"
description = "Take two StringArray and perform the selected Set operation on the arrays."
categories = ["Playbook Apps"]
viewLink = "https://github.com/ThreatConnect-Inc/threatconnect-playbooks/tree/master/apps/TCPB_-_Array_Set_Operations"
+++

# Release Notes
## 1.0.0
* Initial Release

---

# Summary
This playbook App will take two StringArray and perform the selected Set operation on the arrays.

![Info](/post/playbook-apps/images/info-array-set-operations.png)

## Operations
* Is Subset - test whether every element in set A is in set B.
* Is Superset - test whether every element in set A is in set B.
* Union - new set with elements from both set A and set B.
* Intersection - new set with elements common to set A and set B.
* Difference - new set with elements in set A but not in set B.
* Symmetric Difference - new set with elements in either set A or Set B but not both.

# Dependencies
* tcex>=0.7,<0.8

# Input Definitions
* Set A - The first StringArray (set A).
* Set B - The second StringArray (set B).
* Operation - The operation to perform on the StringArray (sets).

![Inputs](/post/playbook-apps/images/input-array-set-operations.png)

# Output Definitions
* array.set.boolean (String) - A boolean value when operation is "Is Subset" or "Is Superset" (e.g., true or false).
* array.set.results (StringArray) - The resulting values from the operation (Union, Intersection, Difference, and Symmetric Difference) between the two sets.
* array.set.count - The number of results in `set.results`.

![Outputs](/post/playbook-apps/images/output-array-set-operations.png)

# Building

```
pip install tcex
tclib
tcpackage
```

# Local Testing

All the environment variables in `tcex.d/profiles/array_set_operations.json` file must be set on the local system.

```
tcrun --group qa-build
```
