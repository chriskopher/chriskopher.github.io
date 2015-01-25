---
layout: page
title: Projects
---

<div class="post">
{% for post in site.posts %}
    <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>

    <span class="post-date">{{ post.date | date_to_string }}</span>
    {{ post.content }}
{% endfor %}
</div>