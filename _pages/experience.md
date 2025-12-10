---
title: "Experience"
permalink: /experience/
layout: single
author_profile: true
---

Below is a selection of my research and industry experience.

{% assign exps = site.experience | sort: "date" | reverse %}
{% for e in exps %}
- [**{{ e.title }}**]({{ e.url | relative_url }})  
  *{{ e.role }} — {{ e.organization }} ({{ e.dates }})*
{% endfor %}
