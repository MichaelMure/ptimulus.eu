---
layout: page
title_key: ptimulus1.galleries_section
permalink: /ptimulus1/galleries/
section: ptimulus1
---

{% for gallery in site.data.galleries %}
  {% if gallery.embedded != true %}
  - [{{ gallery.description }}]({{ gallery.id }})
  {% endif %}
{% endfor %}
