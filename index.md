---
layout: default
title: Home
---

# Kushagra Garg

Researcher in quantum algorithms. Currently at Fujitsu Research Quantum Lab, working on Lindbladian simulation algorithms and quantum resource estimation. Pursuing M.S. in Computational Natural Science at IIIT Hyderabad, focusing on quantum computation, error correction, and variational algorithms.

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
