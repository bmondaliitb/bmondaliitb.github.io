---
title: Research
intro: Calorimeter reconstruction, machine learning, and top-quark physics with ATLAS.
---

## Ongoing

{% assign ongoing = site.research | where: "status", "Ongoing" | sort: "order" %}
<div class="research-grid">
{% for item in ongoing %}{% include research-card.html item=item %}{% endfor %}
</div>

## Past research

{% assign past = site.research | where: "status", "Completed" | sort: "order" %}
<div class="research-grid">
{% for item in past %}{% include research-card.html item=item %}{% endfor %}
</div>
