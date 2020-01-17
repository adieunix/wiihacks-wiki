---
title: Wiki -> Links -> Personality
description: Internet Personalities Related to the Wii.
redirect_from: "/links/personality.md"
---

# Personalities

## ***Disclaimer!***

This information is for archival informational purposes only and does not imply endorsement by r/WiiHacks or WiiHacks.org.

## Blogs

  Sites that host mostly old blogs related to Wii modding.

{% for link in site.data.links_personality.blogs %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Repo Users

  These are the user accounts on repo sites like Github and SourceForge for users that are known to contribute to the Wii Homebrew scene.

{% for link in site.data.links_personality.repo_users %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

## Youtube Channels

  These are YouTube channels of content creators known to create Wii-related content. You might have to search through their sites for Wii specific content.

{% for link in site.data.links_personality.youtube_channels %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}

