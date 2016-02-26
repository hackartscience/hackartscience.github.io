---
layout: page
title: hackartscience
picture-title: https://files.hackartscience.com/export/hackartscience_common/logo/hackartscience.svg
subtitle: here, we can accomplish more together than we could alone
permalink: /
---

{{ site.description }}

some of our featured work:
==========================

{% assign featured_projects = site.projects | where:'featured', true %}
{% for project in featured_projects %}
  {% include project_entry.html %}
{% endfor %}
