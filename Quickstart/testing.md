---
layout: default
title: Testing
nav_order: 2
description: "Testing your watchface"
parent: Quickstart
permalink: /quickstart/testing
---
# Testing your Watchface

Test out your watchface. This guide primarily focuses on m0tral's custom Mi Fitness mod and servers.

{: .no_toc }

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

---

## Prerequisites
There are many ways to transfer watchfaces to your watch. The recommended way is to gain access to @m0tral's watchface database and install your watchface through there. You may like to follow these steps in advance; they make take a while.

{: .info }
The modded Mi Fitness app is only available on Android.

{: .info }
> If you are running Android >13 and get the "Restricted setting" popup, you will need to unlock application permissions.
>
> 1. Open the apps list in settings (Settings > Apps > Show all apps/Settings > Apps > App Management) 
> 2. Choose Mi Fitness from the list
> 3. Tap on the top right corner menu (3 dots)
> 4. Select "Allow restricted settings"

1. Download the modded Mi Fitness APK on Telegram: https://t.me/mi_watch_int by messaging @mi_watch_bot "/latestapp"
2. In the app, open the "Device" tab and tap "About device" (at the bottom of the menu)
3. Copy the MAC address, and message @m0tral on Telegram for access to the development servers with your MAC address.

---

## Testing your Watchface

{: .warning }
> **You may brick your device testing out custom watchfaces.** If your watch does not have 
> good recovery, you risk breaking your watch entirely. Some watches with known bad
> recovery/no recovery:
>
> - Xiaomi Smart Band 8
> - Xiaomi Watch S1 Pro
> - Xiaomi Watch S3
> - Redmi Watch 3
>
> However, watches that run NuttX (Xiaomi Vela/RW4 HyperOS) have really good recovery. 
> You do not need to worry about bricking your device unless you have messed with system
> software. The following devices run NuttX:
>
> - Xiaomi Smart Band 8 Pro
> - Redmi Watch 4
>
> There are some strategies to prevent bricking your watch, listed later on.

Once you're ready to test out your watchface, you can build/compile it to a format that is readable by the watch. To build your watchface:

1. In the toolbar, select the ![Build](../Images/package.png) build button
2. In the popup that appears, fill the following fields:
   - Watchface name - The name of the watchface that appears in the watch
   - Watchface thumbnail - The thumbnail of the watchface that appears in the watch
3. The watchface will be built using the data that is saved **in the project files**, not in the application. You can choose whether to:
   - Save - Save open project to file before building
   - Discard - Dont save anything to file before building
4. Check build results for any errors.

Your watchface binary will be in the output folder in your project.

---

## Debugging

There may have been some watchface errors that slipped through build errors. These errors may brick your device. A way to check for these errors is to unpack the watchface, if any errors occur from unpacking there may have been a bug in your watchface. Please report these bugs to the Mi Watch Development group on Telegram for further assistance.

---

## Transferring to your watch
{ .info}
The .FACE file is your watchface binary. Rename it to .bin if you are uploading to another service.

If you have access to the @m0tral's development servers, access the admin panel at https://miwatch.conversmod.ru/micolor/facemain?YOUR-MAC-ADDRESS-HERE and upload your watchface on the bottom panel. You can apply it in Mi Fitness > Watchfaces > Categories > Test RU 

![category button](../Images/app-categories.jpg)

[Publishing your Watchface >](https://ooflet.github.io/docs/quickstart/publishing){: .btn .btn-blue }