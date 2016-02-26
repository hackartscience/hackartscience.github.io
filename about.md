---
layout: page
title: About Us
subtitle: We are people, and we do things!
permalink: /about/
---

{{ site.description }}

You may send all inquiries to [hi@hackartscience.com](mailto:hi@hackartscience.com), or find us on [social media](#bottom).

Here are a few of us:
====================

{% assign people = site.people | sort: 'order' %}
{% for person in people %}
  {% include person_entry.html %}
{% endfor %}

The rest of us are a little shy, but make ourselves known by contributing to our projects and articles.
