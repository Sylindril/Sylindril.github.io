---
layout: page
title: scientific
permalink: /scientific/
description: Scientific and research writing by Aditya Kumar.
nav: true
nav_order: 2
---

Research notes and essays on agents, learning, interpretability, and automated
scientific discovery.

{% assign scientific_posts = site.categories.scientific %}
{% if scientific_posts.size > 0 %}

<ul class="post-list">
  {% for post in scientific_posts %}
    {% assign read_time = post.content | number_of_words | divided_by: 180 | plus: 1 %}
    <li>
      <h3><a class="post-title" href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.description }}</p>
      <p class="post-meta">{{ read_time }} min read &nbsp; · &nbsp; {{ post.date | date: "%B %d, %Y" }}</p>
    </li>
  {% endfor %}
</ul>

{% else %}

Nothing published here just yet.

{% endif %}
