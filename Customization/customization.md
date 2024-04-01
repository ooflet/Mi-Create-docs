---
layout: default
title: Customization
nav_order: 4
description: "Introduction to Mi Create"
permalink: /customization
---

# Customizing Mi Create

Mi Create has a very modular theming system, allowing for custom but powerful themes to be created.

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

## Theme Components 

A theme consists of 3 things:
- Icons
- Stylesheet
- Color Schemes

Icons use the Free Desktop icon theme specification (https://specifications.freedesktop.org/icon-theme-spec/icon-theme-spec-latest.html). View the default icon theme for an example.

Mi Create uses Qt. Stylesheets are how QWidgets are styled in the application. You may read on how Stylesheets work at https://doc.qt.io/qt-6/stylesheet.html, https://doc.qt.io/qt-6/stylesheet-reference.html

Color Schemes are defined by colorSchemes.json. The name of the scheme is a key and contained are 2 ColorGroups: 
- Base
- Disabled

In the respective ColorGroup, are a list of QPalette ColorRoles, listed at https://doc.qt.io/qt-6/qpalette.html#ColorRole-enum

A combination of these 3 things can help style Mi Create to however you like. 