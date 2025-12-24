---
layout: page
title: Case Studies
permalink: /case-studies/
---

{% assign items = site.case_studies | sort: "order" %}

<ul>
  {% for cs in items %}
    <li style="margin-bottom: 1rem;">
      <a href="{{ cs.url | relative_url }}"><strong>{{ cs.title }}</strong></a>
      {% if cs.summary %}<div>{{ cs.summary }}</div>{% endif %}
    </li>
  {% endfor %}
</ul>
