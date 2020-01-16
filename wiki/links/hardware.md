---
title: Wiki -> Links -> Hardware
description: Related to the Hardware of the Wii.
redirect_from: "/links/hardware.md"
---

# Hardware

  Any links related to the Wii's hardware.

{% for link in site.data.links_hardware %}
  * [{{ link.name }}]({{ link.url }}) - {{ link.description }}
{% endfor %}
