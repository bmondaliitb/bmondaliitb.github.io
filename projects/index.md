---
title: Random projects
kicker: Software outside the collaboration
intro: Focused experiments in scientific tooling, desktop software, literature, and everyday computing. Each page is written in Markdown and can grow with the project.
---

{% assign sorted_projects = site.projects | sort: "order" %}
<div class="card-grid">
{% for item in sorted_projects %}{% include project-card.html item=item %}{% endfor %}
</div>

These are selected, substantive projects found in the sibling `hobby` workspace. Small data folders, generated artwork, virtual environments, and this website itself are intentionally not presented as standalone projects.
