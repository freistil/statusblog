---
layout: page
title: Overview
header: This is Jekyll-Bootstrap
---

## Open Incidents

{% for post in site.posts %}
{% if post.status == 'open' %}
<article>
{{ post.date | date_to_string }} &raquo; <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>

{{ post.content }}
</article>
{% endif %}
{% endfor %}

## Closed Incidents
<ul class="status">
  {% for post in site.posts %}
    {% if post.status == 'closed' %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
