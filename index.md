---
layout: default
title: Home
---

Hi there! I'm a Research Scientist at [Fujitsu Research](https://global.fujitsu/en-apac/local/technology/research), where I focus on developing quantum algorithms for efficient simulation of open quantum systems.

Before this, I was fortunate to spend time at Microsoft Research, where I worked with [Nishanth Chandran](https://www.microsoft.com/en-us/research/people/nichandr/) on applying cryptography to enable secure inference for Large Language Models.

I completed my Master's at IIIT Hyderabad, where I explored quantum algorithms for intermediate-term quantum devices, advised by [Shantanav Chakraborty](https://sites.google.com/view/shchakra) and [Subhadip Mitra](https://sites.google.com/site/subhadipmitra/).

## Publications

{% for pub in site.data.publications %}
{{ forloop.index }}. {{ pub.authors | replace: "K. Garg", "**K. Garg**" }}. "{{ pub.title }}." *{{ pub.venue }}*, {{ pub.year }}. {% if pub.arxiv %}[arXiv:{{ pub.arxiv }}](https://arxiv.org/abs/{{ pub.arxiv }}){% endif %} {% if pub.doi %}[DOI]({{ pub.doi }}){% endif %}
{% endfor %}

## Contact

**Email:** kushargsg@gmail.com

Feel free to reach out for research collaborations, discussions, or just to say Hi!

