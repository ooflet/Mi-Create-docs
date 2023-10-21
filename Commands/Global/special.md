---
layout: default
title: Special
nav_order: 3
description: "Special"
parent: Commands
permalink: /commands/special
---


# Special
Special mode is dedicated for running modules, Kommand library commands, and custom scripts to be used with Kommand.

{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

## Summary
### module

| `install <moduleName>`                                                                     |
| :----------------------------------------------------------------------------------------- |
| Installs and runs the module from the Kommand repositories with the provided `moduleName`. |

| `installfromlink <moduleLink>`                    |
| :------------------------------------------------ |
| Installs and runs the module from `<moduleLink>`. |

---
## module
These commands technically come under the `module` library, although you run these command straight up.

### `install <moduleName>`
Installs and runs the module from the Kommand's Git repositories with the provided `moduleName`. **Names are case sensitive.**
```
install InfiniteYield
```

### `installfromlink <moduleLink>`
Installs and runs the module from the link provided.
```
installfromlink https://raw.githubusercontent.com/ooflet/kommand/main/modules/InfiniteYield.kmd
```

