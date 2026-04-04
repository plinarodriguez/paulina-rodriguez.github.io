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
<!-- <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %} -->

<div class="repo-card p-3 mb-3 border rounded">
  <a href="https://github.com/{{ include.repository }}">
    <h5 class="mb-1">{{ include.repository }}</h5>
  </a>
  <p class="mb-1 small text-muted">
    {{ include.description | default: "GitHub repository" }}
  </p>
</div>


<!-- </div> -->
{% endif %}

---

## GitHub Repositories

{% if site.data.repositories.github_repos %}
<!-- <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %} -->
<div class="repo-card p-3 mb-3 border rounded">
  <a href="https://github.com/{{ include.username }}">
    <h5>@{{ include.username }}</h5>
  </a>
</div>

<!-- </div> -->
{% endif %}
