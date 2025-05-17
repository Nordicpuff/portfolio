---
layout: page
title: Updates
permalink: /updates/
---

<ul class="post-list">
{% for update in site.updates reversed %}
    <li>
        <h2><a class="update-title" href="{{ update.url | prepend: site.baseurl }}">{{ update.title }}</a></h2>
        <p class="post-meta">{{ update.date | date: '%B %-d, %Y — %H:%M' }}</p>
        <img src="{{ update.img }}" style="width:300px;">
    </li>
{% endfor %}
</ul>