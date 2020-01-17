---
title: Wiki -> Links -> Software
description: Software related to Wii Modding.
redirect_from: "/links/software.md"
---

# Software for the Wii

  Various Software for the Wii, broken down into three categories:

## ***WARNING!***

  Some of the software on this page can damage your Wii. Please know what you are doing before you utilize it.

## Emulators

  Here you will find links to emulators for the Wii and articles related to using them.

{% for link in site.data.links_software.emulators %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Loaders

  This section is for software that loads other software either onto your Wii's long-term storage, or into memory to run.

{% for link in site.data.links_software.loaders %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Modding/Utility

  This is software directly related to modding your Wii, or interacting with your Wii system.

{% for link in site.data.links_software.utility %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

