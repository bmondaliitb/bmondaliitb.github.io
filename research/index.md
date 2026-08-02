---
title: Research
kicker: What I work on
intro: From calorimeter signals to top-quark measurements, my work is about extracting robust physics from a complex detector environment.
---

{% assign ongoing = site.research | where: "status", "Ongoing" | sort: "order" %}
<div class="research-grid">
{% for item in ongoing %}{% include research-card.html item=item %}{% endfor %}
</div>

## Past research

{% assign past = site.research | where: "status", "Completed" | sort: "order" %}
<div class="research-grid">
{% for item in past %}{% include research-card.html item=item %}{% endfor %}
</div>
