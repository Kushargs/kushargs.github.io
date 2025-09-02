---
layout: default
title: Home
---

# Kushagra Garg

Researcher in quantum algorithms. Exploring quantum information, computational complexity, and machine learning applications in quantum systems. Currently pursuing research at the intersection of quantum computation and optimization.

## Links

- [GitHub](https://github.com/kushargs)
- [CV](/cv/kushagra_cv.pdf)
- [Email](mailto:kushargsg@gmail.com)
- [Google Scholar](https://scholar.google.com/citations?user=yourid)

## Publications

{% for pub in site.data.publications %}
{{ forloop.index }}. **{{ pub.authors }}**. "{{ pub.title }}." *{{ pub.venue }}*, {{ pub.year }}. {% if pub.arxiv %}[arXiv:{{ pub.arxiv }}](https://arxiv.org/abs/{{ pub.arxiv }}){% endif %} {% if pub.doi %}[DOI]({{ pub.doi }}){% endif %}
{% endfor %}

## Selected Talks

{% for talk in site.data.talks %}
- **{{ talk.title }}** - {{ talk.venue }}, {{ talk.date }}
{% endfor %}
