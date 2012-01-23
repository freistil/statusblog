---
layout: page
title: Current status at freistil IT
header: This is Jekyll-Bootstrap
---

## Open incidents

{% for post in site.posts %}
{% if post.status == 'open' %}
<article>
<span class="status_date">{{ post.date | date_to_string }}</span>
<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>

{{ post.content }}
</article>
{% endif %}
{% endfor %}

## Resolved incidents
<ul class="status">
  {% for post in site.posts %}
    {% if post.status == 'resolved' %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
