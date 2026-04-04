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
  <p class="mb-1 small text-muted">
    <h5>
      {% for user in site.data.repositories.github_users %}
        {% include repository/repo_user.html username=user %}
      {% endfor %}
    </h5>
  </p>
</div>
{% endif %}

---

## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repo-card p-3 mb-3 border rounded">
    <h5>
    {% for repo in site.data.repositories.github_repos %}
      {% include repository/repo.html repository=repo %}
    {% endfor %} 
    </h5>
</div>
{% endif %}

