---
layout: default
title: Contributing
nav_order: 5
description: "Contributing to Mi Create"
permalink: /contribute
---
# Contribute to Mi Create

Thank you for your interest in contributing to Mi Create! 

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

## Translations

{ .info }
You can view a list of language codes at https://en.wikipedia.org/wiki/List_of_ISO_639_language_codes 

Currently, translations are done using GNU's gettext standard. To edit existing translations, clone the repository, open the locales folder in src/locales, open your locale's folder > LC_MESSAGES and edit using a program like Poedit:

- main.po - Strings in main.py
- properties.po - Strings in properties
- window.po - Strings in precompiled window

To create a translation entry, create a folder with your language code (you could name this folder anything but to keep standards please name it to a language code). In the folder, create a CONFIG.ini file. This file contains the configuration details of your language:

> [config]  
> language = Language Name  
> authorMessage = Comment  
> contact = Contact Details  

Once config files have been created, using a program like Poedit, create your translation files from the pot files in /locales.

---

## Funding

I am not accepting donations for Mi Create. Treat the project as a community effort.