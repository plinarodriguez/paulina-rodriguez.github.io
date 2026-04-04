---
layout: page
permalink: /repositories/
title: repositories
description: Here are my current GitHub profiles and repositories
nav: true
nav_order: 4
---



## GitHub users

{% if site.data.repositories.github_users %}
<div class="repo-card p-3 mb-3 border rounded">
  <a href="https://github.com/{{ include.repository }}">
    <h5 class="mb-1">{{ include.repository }}</h5>
  </a>
  <p class="mb-1 small text-muted">
    {{ include.description | default: "GitHub repository" }}
  </p>
</div>
{% endif %}

---

## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repo-card p-3 mb-3 border rounded">
  <a href="https://github.com/{{ include.username }}">
    <h5>@{{ include.username }}</h5>
  </a>
</div>
{% endif %}

