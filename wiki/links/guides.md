---
title: Wiki -> Links -> Guides
description: All guides Wii-related
redirect_from: "/links/guides.md"
---

## Web Based / Print Tutorials

{% for link in site.data.links_guides.web %}
{% if link.piracy == false %}
#### [{{ link.name }}]({{ link.url }})

Date: {{ link.date }}
{% if link.description != '' %}

- {{ link.description }}
{% endif %}
{% endif %}
{% endfor %}

## Youtube Tutorials

{% for link in site.data.links_guides.youtube %}
{% if link.piracy == false %}
#### [{{ link.name }}]({{ link.url }})

Date: {{ link.date }}
{% if link.description != '' %}

- {{ link.description }}
{% endif %}
{% endif %}
{% endfor %}
