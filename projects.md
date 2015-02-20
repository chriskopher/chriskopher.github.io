---
layout: page
title: Projects
---

<p class="message">
  Here are my personal projects. Have a look around! I'll be keeping the posts up-to-date.
</p>

<div class="post">
{% for post in site.posts %}
    <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>

    <span class="post-date"> {{ post.start | date: "%-d %B %Y" }}
    &#8212 {{ post.end | date: "%-d %B %Y" }} </span>

    {{ post.excerpt }}
{% endfor %}
</div>
