---
layout: page
title: Home
full_width: true
---
<section class="hero">
  <div class="shell">
    <p class="eyebrow">Particle physics · Prague & CERN</p>
    <h1>Buddhadeb Mondal</h1>
    <p class="lede">I’m a postdoctoral researcher at FZU, working on the ATLAS experiment at CERN. I study calorimeter reconstruction, machine learning, and precision top-quark measurements.</p>
    <div class="button-row">
      <a class="button" href="{{ '/research/' | relative_url }}">Research <span aria-hidden="true">→</span></a>
      <a class="button button--secondary" href="{{ '/CV_Buddhadeb_Mondal.pdf' | relative_url }}">CV (PDF)</a>
    </div>
  </div>
</section>

<section class="section">
  <div class="shell">
    <div class="section-heading">
      <h2>Selected research</h2>
      <a href="{{ '/research/' | relative_url }}">All research <span aria-hidden="true">→</span></a>
    </div>
    <ul class="selected-research">
      {% assign selected = site.research | where: "featured", true | sort: "order" %}
      {% for item in selected limit:3 %}
      <li>
        <a href="{{ item.url | relative_url }}">{{ item.title }}</a>
        <span class="period">{{ item.period }}</span>
      </li>
      {% endfor %}
    </ul>
  </div>
</section>

<section class="section">
  <div class="shell about-strip">
    <h2>Background</h2>
    <div>
      <p>I completed my PhD at the University of Siegen. My ATLAS work has covered pixel data-acquisition software, data-driven background estimates, and differential measurements of top-quark-pair production with a photon.</p>
      <a href="{{ '/cv/' | relative_url }}">Experience, education, and talks <span aria-hidden="true">→</span></a>
    </div>
  </div>
</section>
