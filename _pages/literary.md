---
layout: page
title: literary
permalink: /literary/
description: Poetry and literary writing by Aditya Kumar.
nav: true
nav_order: 1
---

Poetry, personal essays, theatre, history, cinema, and other attempts at
tasteful prose.

{% assign literary_posts = site.categories.literary %}
{% if literary_posts.size > 0 %}

<ul class="post-list">
  {% for post in literary_posts %}
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
