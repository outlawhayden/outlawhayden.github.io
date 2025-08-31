---
layout: page
permalink: /repositories/
title: repositories
description: Active and past projects on github, as well as my personal profile. 
nav: true
nav_order: 3
---
## Languages

I predominantly build in Python, but am familiar to a lesser extent with Rust, MATLAB, C++, and Java. I also have experience in Javascript, React, HTML/CSS, Julia, Haskell, NetLogo, and OCaml.
---


{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>
{% endif %}

---

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
