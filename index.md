---
layout: page
title: Current status at freistil IT
header: This is Jekyll-Bootstrap
---

<div class="alert alert-info">
To get maintenance announcements and other important information directly to your mailbox, please [subscribe to our Operations Newsletter](https://tinyletter.com/freistilops)!
</div>

## Open incidents

{% for post in site.posts %}
{% if post.status == 'open' %}
{% assign open_exists = true %}
<article class="status front">
<span class="severity {{ post.severity }}"> </span>
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
