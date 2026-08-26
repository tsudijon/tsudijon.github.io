---
layout: archive
title: "Notes"
permalink: /notes/
author_profile: true
---

{% include base_path %}

{% assign notes = site.notes | sort: "date" | reverse %}

{% if notes.size > 0 %}
  {% for post in notes %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
Notes coming soon.
{% endif %}
