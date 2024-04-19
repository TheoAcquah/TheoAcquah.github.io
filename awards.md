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
    {% if award.image_paths %}
      {% for image_path in award.image_paths %}
        <img src="{{ site.baseurl }}/images/{{ image_path }}" alt="{{ award.title }} Image" style="max-width: 100%; height: auto;">
      {% endfor %}
    {% endif %}
  </li>
{% endfor %}
</ul>
