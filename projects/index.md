---
title: Projects
intro: Software I build outside my research.
---

{% assign sorted_projects = site.projects | sort: "order" %}
<div class="card-grid">
{% for item in sorted_projects %}{% include project-card.html item=item %}{% endfor %}
</div>
