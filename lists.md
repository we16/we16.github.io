---
layout: page
permalink: /lists/
title: lists
description: Just like the title says. A bunch of lists of things.
---

<ul class="post-list">
{% for list in site.lists reversed %}
    <li>
        <h2><a class="list-title" href="{{ list.url | prepend: site.baseurl }}">{{ list.title }}</a></h2>
        <p class="post-meta">{{ list.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>