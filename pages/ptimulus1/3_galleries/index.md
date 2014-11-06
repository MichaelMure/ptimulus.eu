---
layout: page
title: Galeries photos
permalink: /ptimulus1/galleries/
section: ptimulus1
---

{% for gallery in site.data.galleries %}
  {% if gallery.embedded != true %}
  - [{{ gallery.description }}]({{ gallery.id }})
  {% endif %}
{% endfor %}
