---
layout: page
title: Volunteer
---

<p class="message">
  These are my volunteer activities. Let me know if you're looking for a helping hand!
</p>

<div class="post">
{% for post in site.tags.volunteer %}            <!--- filters page to only show tags: volunteer --->

<h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>

<span class="post-date"> {{ post.start | date: "%-d %B %Y" }}
&#8212 {{ post.end | date: "%-d %B %Y" }}
</span>

{{ post.excerpt }}
{% endfor %}
</div>
