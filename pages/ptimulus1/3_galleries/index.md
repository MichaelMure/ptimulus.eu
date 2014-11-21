---
layout: page
title_key: ptimulus1.galleries_section
permalink: /ptimulus1/galleries/
section: ptimulus1
---

{% assign pages = site.pages | sort:"path"  %}
{% for site_page in pages %}
  {% if site_page.subsection == 'galleries' and site_page.section == 'ptimulus1' %}
  {% capture full_title_key %}title.{{ site_page.title_key }}{% endcapture %}
  - <a href="{{site.baseurl}}{{ site_page.url }}">{% t full_title_key %}</a>
  {% endif %}
{% endfor %}