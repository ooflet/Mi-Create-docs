---
layout: default
title: Prefix
nav_order: 2
description: "Prefix"
parent: Quickstart
permalink: /quickstart/prefix
---
# Prefix
{: .no_toc }
Prefixes are your main way of interacting with Kommand. They show which mode the command will be running in. In order to change your prefix, **Press the character whilst in an empty command bar**. 

---
## Prefix list

| Prefix | No.  | Description                                                  |
| :----- | :--- | :----------------------------------------------------------- |
| >      | 0    | Execute mode, runs Lua code                                  |
| *      | 1    | System mode, modify and run system commands                  |
| !      | 3    | Special mode, run custom modules and default library modules |
| ?      | 2    | Help mode, run help wizard commands                          |

---

## Notes

- You may manually change the mode by going into system mode and running `debug  setcurrentmode <modeNumber>`.
