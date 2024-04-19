---
layout: default  # or any other layout
title: Awards
permalink: /awards/
---

<h1>Awards</h1>
<ul>
{% for award in site.data.awards %}
  <li>
    <strong>{{ award.year }}</strong>: {{ award.title }}, {{ award.event }} ({{ award.organization }})
    <br>
    <img src="{{ site.baseurl }}/images/{{ award.url }}" alt="Award Image">
  </li>
{% endfor %}
</ul>

