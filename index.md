---
layout: page
title: Home
full_width: true
---
<section class="home-intro">
  <div class="shell home-intro-grid">
    <div>
      <h1>Particle physicist</h1>
      <p>I’m a postdoctoral researcher at FZU in Prague, working on the ATLAS experiment at CERN. I study calorimeter reconstruction, machine learning, and precision top-quark measurements.</p>
    </div>
    <div class="home-background">
      <h2>Background</h2>
      <p>I completed my PhD at the University of Siegen. My ATLAS work has covered pixel data-acquisition software, data-driven background estimates, and differential measurements of top-quark-pair production with a photon.</p>
      <p class="home-cv-links"><a href="{{ '/cv/' | relative_url }}">Experience and talks</a> · <a href="{{ '/CV_Buddhadeb_Mondal.pdf' | relative_url }}">CV (PDF)</a></p>
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
        <span class="period">{{ item.status }} · {{ item.period }}</span>
      </li>
      {% endfor %}
    </ul>
  </div>
</section>
