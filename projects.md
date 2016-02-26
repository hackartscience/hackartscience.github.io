---
layout: page
title: Projects
subtitle: Here is where the lasting things we tinker on live
permalink: /projects/
---

{% for project in site.projects %}
  {% include project_entry.html %}
{% endfor %}
