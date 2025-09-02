---
layout: default
title: Blog
---

# Blog

{% for post in site.posts %}
<article>
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
  {{ post.excerpt }}
</article>
{% endfor %}
