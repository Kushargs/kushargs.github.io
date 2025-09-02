---
layout: default
title: Home
---

# Your Name

Researcher in quantum algorithms. PhD student exploring quantum information, complexity, and machine learning applications.

## Links

- [GitHub](https://github.com/yourusername)
- [CV](/cv/yourname_cv.pdf)
- [Email](mailto:you@example.com)
- [Google Scholar](https://scholar.google.com/citations?user=yourid)

## Publications

{% for pub in site.data.publications %}
{{ forloop.index }}. **{{ pub.authors }}**. "{{ pub.title }}." *{{ pub.venue }}*, {{ pub.year }}. {% if pub.arxiv %}[arXiv:{{ pub.arxiv }}](https://arxiv.org/abs/{{ pub.arxiv }}){% endif %} {% if pub.doi %}[DOI]({{ pub.doi }}){% endif %}
{% endfor %}

## Selected Talks

{% for talk in site.data.talks %}
- **{{ talk.title }}** - {{ talk.venue }}, {{ talk.date }}
{% endfor %}
