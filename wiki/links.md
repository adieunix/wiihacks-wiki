---
title: Wiki -> Links
description: A wiki maintained by the r/WiiHacks community.
redirect_from: "/links.md"
---

# Useful Links Intro:

  These links will help you get the most out of your Wii. From useful to interesting.

# ***WARNING!***

  * There is a lot of software listed that is old and no longer used. Please make sure you know what you're doing before you attempt to use any software you aren't familiar with. 
  * There are youtuber's and youtube tutorials listed which are known to cause issues when their videos are followed. Please do your research before using them.

## Blogs

  Sites that host mostly old blogs related to Wii modding.

{% for link in site.data.links.blogs %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Communities

  Here is a list of communities that are somehow related to the Wii.

{% for link in site.data.links.communities %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Games, Game Mods, and Game Related Sites

  Anything game related, game modding related, etc.

{% for link in site.data.links.games %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Hardware related

  Any links related to the Wii's hardware.

{% for link in site.data.links.hardware %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Reference Articles

  These articles are listed for quick reference. Note that they might be contained within sites listed elsewhere on this page.

{% for link in site.data.links.references %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Repo Users

  These are the user accounts on repo sites like Github and SourceForge for users that are known to contribute to the Wii Homebrew scene.

{% for link in site.data.links.repo_users %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Software for the Wii

  Various Software for the Wii, broken down into three categories:

### Emulators

  Here you will find links to emulators for the Wii and articles related to using them.

{% for link in site.data.links.software.emulators %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

### Loaders

  This section is for software that loads other software either onto your Wii's long-term storage, or into memory to run.

{% for link in site.data.links.software.loaders %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

### Modding/Utility

  This is software directly related to modding your Wii, or interacting with your Wii system.

{% for link in site.data.links.software.utility %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Themes and theme related links

  Anything and everything related to theming your Wii. Please be warned that changing system menu attributes has been a common cause for bricked Wiis.

{% for link in site.data.links.themes %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Youtube Channels

  These are YouTube channels of content creators known to create Wii-related content. You might have to search through their sites for Wii specific content.

{% for link in site.data.links.youtube_channels %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Notes:

  There's so much that needs to be added to this to make it complete. Please don't hesitate to drop us a line to add to this list.

  If you moderate any of the above links, and would like more recognition or collaboration ...

  ... or if you'd like to add a a link or report a broken link please feel free to contact the moderators via modmail.