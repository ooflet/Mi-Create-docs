---
layout: default
title: System
nav_order: 2
description: "System"
parent: Commands
permalink: /commands/system
---

# System
System commands are usually commands to modify Kommand. They use the `*` prefix

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
### settings

| `settings blur <bool>`                     |
| :----------------------------------------- |
| Shows or hides the background blur effect. |

### debug

| `debug setcurrentmode <modeNumber>`                |
| :------------------------------------------------- |
| Changes the current mode (prefix) to `modeNumber`. |

### Miscellaneous

| `console`                                        |
| :----------------------------------------------- |
| Toggles to the default Roblox Developer Console. |

| `safehop`/`serverhop`                                                       |
| :-------------------------------------------------------------------------- |
| Quickly disconnects and teleports the user into another server in the game. |

| `exit`                          |
| :------------------------------ |
| Entirely closes out of Kommand. |

---

## settings
These commands modify or change Kommand's settings. The setting.json file can be found at `/workspace/Kommand/settings/setting.json`

### `blur <SettingsBlurValue>`
Shows or hide the background blur effect. This can be manually changed by changing the `blur` value in `setting.json`. Values can be true, false, or auto.
```
settings blur false
```

---

## debug
These commands are used for debugging purposes.

### `setcurrentmode <modeNumber>`
Sets the current mode or prefix to `modeNumber`. Mode numbers can be found [here](https://ooflet.github.io/docs/quickstart/prefix).
```
debug setcurrentmode 1
```
---

## Miscellaneous

### `safehop`/`serverhop`
Quickly & safely kicks the player out of the current server and teleports them into another server in the game.

### `exit`
Entirely closes out of Kommand. To simply hide the Kommand terminal press F9 or click the X button on the top right hand corner.
