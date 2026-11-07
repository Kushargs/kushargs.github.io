---
layout: default
title: Kushagra Garg
---
<header class="intro" aria-labelledby="name">
  <div class="intro-copy">
    <h1 id="name">Kushagra Garg</h1>
    <p class="bio">I'm a PhD student in the Department of Computer Science at the University of Toronto, supervised by <a href="https://cqiqc.physics.utoronto.ca/people/cqiqc-members/nathan-wiebe/">Nathan Wiebe</a>. My research interests include quantum algorithms and the simulation of open quantum systems.</p>
    <nav class="profile-links" aria-label="Profile links">
      <a href="mailto:{{ site.email }}">Email</a>
      <a href="{{ site.scholar_link | escape }}">Scholar</a>
      <a href="https://github.com/{{ site.github_username }}">GitHub</a>
      <a href="{{ '/cv/kushagra_cv.pdf' | relative_url }}">CV <span class="file-type">PDF</span></a>
    </nav>
  </div>
  <div class="portrait">
    <img src="{{ '/images/kushagra-portrait.jpeg' | relative_url }}" alt="Kushagra smiling in diving gear" width="800" height="1000" fetchpriority="high">
  </div>
</header>

<div class="background">
  <p>Previously, I worked at Fujitsu Research, Microsoft Research, and QunaSys. I completed my master's at IIIT Hyderabad, advised by <a href="https://sites.google.com/view/shchakra">Shantanav Chakraborty</a> and <a href="https://sites.google.com/site/subhadipmitra/">Subhadip Mitra</a>. My <a href="{{ '/assets/Thesis.pdf' | relative_url }}">master's thesis</a> explores early fault-tolerant quantum algorithms for open quantum systems.</p>
</div>

<section class="publications" aria-labelledby="publications">
  <h2 id="publications">Publications</h2>
  <ul class="publication-list">
    {% for pub in site.data.publications %}
    <li class="publication">
      {% if pub.doi %}{% assign paper_url = pub.doi %}{% else %}{% assign paper_url = 'https://arxiv.org/abs/' | append: pub.arxiv %}{% endif %}
      <h3><a href="{{ paper_url }}">{{ pub.title | escape }}</a></h3>
      <p class="authors">{{ pub.authors | escape | replace: 'K. Garg', '<strong>K. Garg</strong>' }}</p>
      <p class="publication-details"><span class="venue">{{ pub.venue | escape }}</span><span class="separator" aria-hidden="true">·</span>{{ pub.year }}<span class="separator" aria-hidden="true">·</span>{% if pub.doi %}<a href="{{ pub.doi }}" aria-label="Read {{ pub.title | escape }}">Paper <span aria-hidden="true">↗</span></a>{% endif %}{% if pub.arxiv %}{% if pub.doi %}<span class="separator" aria-hidden="true">·</span>{% endif %}<a href="https://arxiv.org/abs/{{ pub.arxiv }}" aria-label="Read {{ pub.title | escape }} on arXiv">arXiv <span aria-hidden="true">↗</span></a>{% endif %}{% if pub.code %}<span class="separator" aria-hidden="true">·</span><a href="{{ pub.code }}">Code <span aria-hidden="true">↗</span></a>{% endif %}</p>
    </li>
    {% endfor %}
  </ul>
</section>

<section class="contact" aria-labelledby="contact">
  <h2 id="contact">Get in touch</h2>
  <p>I'm happy to chat about research and potential collaborations.<br>
    <a href="mailto:{{ site.email }}">{{ site.email }}</a></p>
</section>
