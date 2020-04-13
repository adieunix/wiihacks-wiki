---
title: Wiki -> Rules -> Mod Rules -> Removal Templates
description: Templates to post for removal messages.
redirect_from: "/rules/removal.md"
---

## Why does this exist?

Removal templates are stored in a yml file in the _data directory so they can
be read and written to by the bot. Currently they are being manually 
copy/pasted from the data contained in /_data/template_removals.yml

-----

{% for template in site.data.template_removals %}

### {{ template.title }}

{{ template.body }}

-----
{% endfor %}