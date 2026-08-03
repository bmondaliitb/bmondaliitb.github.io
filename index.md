---
layout: page
title: Home
full_width: true
---
<section class="hero">
  <div class="shell hero-grid">
    <div class="hero-copy">
      <p class="eyebrow">Particle physicist · Prague & CERN</p>
      <h1>Making complex collisions <span>measurable.</span></h1>
      <p class="lede">I am a postdoctoral researcher at FZU, working with the ATLAS experiment at CERN. I study calorimeter reconstruction, machine learning, and precision top-quark measurements.</p>
      <div class="button-row">
        <a class="button" href="{{ '/research/' | relative_url }}">Explore my research</a>
        <a class="button button--secondary" href="{{ '/CV_Buddhadeb_Mondal.pdf' | relative_url }}">Download CV</a>
      </div>
    </div>
    <div class="detector-visual" role="img" aria-label="Abstract cross-section of a particle detector with tracks emerging from a collision">
      <span class="collision"></span>
      <span class="track"></span><span class="track"></span><span class="track"></span><span class="track"></span>
      <span class="detector-label detector-label--a">calorimeter signals</span>
      <span class="detector-label detector-label--b">13 TeV collisions</span>
      <span class="detector-label detector-label--c">precision + ML</span>
    </div>
  </div>
</section>

<section class="section section--surface">
  <div class="shell">
    <div class="section-heading">
      <p class="eyebrow">Research</p>
      <h2>Current research</h2>
      <p>I develop machine-learning methods for ATLAS calorimeter-cluster calibration and study their effects on jets, recoil, and missing transverse momentum.</p>
    </div>
    <div class="research-grid">
      {% assign current_research = site.research | where: "featured", true | sort: "order" %}
      {% for item in current_research limit:3 %}{% include research-card.html item=item %}{% endfor %}
    </div>
    <a class="section-link" href="{{ '/research/' | relative_url }}">See ongoing and past research →</a>
  </div>
</section>

<section class="section section--surface">
  <div class="shell about-strip">
    <div>
      <p class="eyebrow">About</p>
      <h2>Background</h2>
    </div>
    <div>
      <p>I completed my PhD at the University of Siegen, working on the ATLAS experiment. My research has included pixel data-acquisition software, data-driven background estimates, and differential measurements of top-quark-pair production with a photon.</p>
      <div class="fact-list">
        <div class="fact"><strong>FZU</strong><span>Postdoctoral researcher</span></div>
        <div class="fact"><strong>ATLAS</strong><span>CERN collaboration</span></div>
        <div class="fact"><strong>Siegen</strong><span>PhD in particle physics</span></div>
      </div>
      <a class="section-link" href="{{ '/cv/' | relative_url }}">Education, experience, and talks →</a>
    </div>
  </div>
</section>
