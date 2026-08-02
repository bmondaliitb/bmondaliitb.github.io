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
      <p class="lede">I am a postdoctoral researcher at the Institute of Physics of the Czech Academy of Sciences (FZU), working with the ATLAS experiment at CERN. My research connects calorimeter reconstruction, machine learning, and precision measurements of the top quark.</p>
      <div class="button-row">
        <a class="button" href="{{ '/research/' | relative_url }}">Explore my research</a>
        <a class="button button--secondary" href="{{ '/CV_Buddhadeb_Mondal.pdf' | relative_url }}">Download CV</a>
      </div>
    </div>
  </div>
</section>

<section class="section section--surface">
  <div class="shell">
    <div class="section-heading">
      <p class="eyebrow">Current focus</p>
      <h2>Better inputs for better physics.</h2>
      <p>I develop and evaluate machine-learning methods for calibrating ATLAS calorimeter clusters, then study how those improvements propagate to jets, hadronic recoil, and missing transverse momentum.</p>
    </div>
    <div class="research-grid">
      {% assign current_research = site.research | where: "featured", true | sort: "order" %}
      {% for item in current_research limit:4 %}{% include research-card.html item=item %}{% endfor %}
    </div>
    <a class="section-link" href="{{ '/research/' | relative_url }}">See ongoing and past research →</a>
  </div>
</section>

<section class="section">
  <div class="shell">
    <div class="section-heading">
      <p class="eyebrow">Selected software</p>
      <h2>Small tools with a clear job.</h2>
      <p>Outside collaboration work, I build focused desktop and web tools—for visual thinking, Bengali literature, scientific workflows, and the Linux desktop.</p>
    </div>
    <div class="card-grid">
      {% assign featured_projects = site.projects | where: "featured", true | sort: "order" %}
      {% for item in featured_projects limit:6 %}{% include project-card.html item=item %}{% endfor %}
    </div>
    <a class="section-link" href="{{ '/projects/' | relative_url }}">Browse all side projects →</a>
  </div>
</section>

<section class="section section--surface">
  <div class="shell about-strip">
    <div>
      <p class="eyebrow">About</p>
      <h2>Physics, from detector signals to published results.</h2>
    </div>
    <div>
      <p>My path through experimental particle physics began with jet substructure and cosmic-ray anisotropy, continued through ATLAS pixel data-acquisition software and data-driven background estimates, and led to differential measurements of top-quark-pair production with a photon. Today, I work at FZU in Prague on machine-learned calorimeter calibration.</p>
      <div class="fact-list">
        <div class="fact"><strong>ATLAS</strong><span>CERN collaboration</span></div>
        <div class="fact"><strong>140 fb⁻¹</strong><span>Run 2 dataset used in tt̄γ</span></div>
        <div class="fact"><strong>300+</strong><span>ATLAS papers co-authored</span></div>
      </div>
      <a class="section-link" href="{{ '/cv/' | relative_url }}">Education, experience, and talks →</a>
    </div>
  </div>
</section>
