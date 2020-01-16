---
title: Wiki -> WiiDev
description: Development for the Wii
redirect_from: "/wiidev/wiidev.md"
---

# Welcome to r/WiiHack's HomeBrew Development Corner!

Here we've tried to compile enough information to allow anyone to get started with developing homebrew applications on the Wii.

## Getting Started

Here on the [Getting Started](./setup.md) page you will learn the basics on setting up a development environment, and what you either should know, or what you'll be up against learning if you decide to make your own homebrew application.

## Usefull Links

{% for link in site.data.links_development %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}
