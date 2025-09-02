---
layout: default
title: Notes
---

# Notes

{% for link in site.data.links %}
- [{{ link.title }}]({{ link.url }})
{% endfor %}
