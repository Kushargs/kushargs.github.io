---
layout: default
title: Home
---

Researcher in quantum algorithms. Currently at Fujitsu Research Quantum Lab, working on Lindbladian simulation algorithms and quantum resource estimation. Pursuing M.S. in Computational Natural Science at IIIT Hyderabad, focusing on quantum computation, error correction, and variational algorithms.

## Publications

{% for pub in site.data.publications %}
{{ forloop.index }}. {{ pub.authors | replace: "K. Garg", "**K. Garg**" }}. "{{ pub.title }}." *{{ pub.venue }}*, {{ pub.year }}. {% if pub.arxiv %}[arXiv:{{ pub.arxiv }}](https://arxiv.org/abs/{{ pub.arxiv }}){% endif %} {% if pub.doi %}[DOI]({{ pub.doi }}){% endif %}
{% endfor %}

## Contact

**Email:** kushargsg@gmail.com

Feel free to reach out for research collaborations, discussions about quantum computing, or any questions about my work.

