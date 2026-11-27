---
layout: academic
title: "Research & publications"
permalink: /publications/
author_profile: false
---

<div class="shell document-page">
<header class="document-header">
  <p class="eyebrow">Research</p>
  <h1>Research &amp; publications</h1>
  <p>Understanding perception through psychophysics, neural measurements, and computational models.</p>
</header>

<div class="document-content">
  <h2>Research themes</h2>

  <section class="education-entry">
    <h3>Primate visual perception</h3>
    <p>Computational models of figure–ground perception and edge detection, supported by visual psychophysics and optical imaging of macaque V1 at The University of Texas at Austin.</p>
  </section>

  <section class="education-entry">
    <h3>Multisensory inference</h3>
    <p>Bayesian causal inference of audiovisual localization, investigated during my psychology studies in the Landy Lab at New York University.</p>
  </section>

  <section class="education-entry">
    <h3>Perceptual organization</h3>
    <p>Perceptual grouping in visual crowding, the subject of my undergraduate thesis at Jilin University.</p>
  </section>

  <h2>Publications</h2>
  {% assign listed_publications = site.publications | where_exp: "paper", "paper.published != false" | sort: "date" | reverse %}
  {% if listed_publications.size > 0 %}
    <div class="publication-list">
      {% for paper in listed_publications %}
      <article class="publication-entry">
        <h3><a href="{{ paper.url | relative_url }}">{{ paper.title }}</a></h3>
        {% if paper.citation %}<p>{{ paper.citation }}</p>{% endif %}
        {% if paper.paperurl %}<a class="text-link" href="{{ paper.paperurl }}">Read the paper <span aria-hidden="true">↗</span></a>{% endif %}
      </article>
      {% endfor %}
    </div>
  {% else %}
    <p>For publication and manuscript details, please <a href="mailto:{{ site.author.email }}">get in touch</a>.</p>
  {% endif %}
</div>

</div>
