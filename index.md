---
layout: page
title: Current status at freistil IT
header: This is Jekyll-Bootstrap
---

## Open incidents

{% for post in site.posts %}
{% if post.status == 'open' %}
{% assign open_exists = true %}
<article class="status">
<span class="status_date">&raquo; {{ post.date | date_to_string }}</span>

<h3 style="display: inline;"><a href="{{ post.url }}">{{ post.title }}</a></h3>

{{ post.content }}
</article>
{% endif %}
{% endfor %}

{% if open_exists != true %}
<div id="noproblems">No known problems.</div>
{% endif %}

## Resolved incidents
<ul class="status">
  {% for post in site.posts %}
    {% if post.status == 'resolved' %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
