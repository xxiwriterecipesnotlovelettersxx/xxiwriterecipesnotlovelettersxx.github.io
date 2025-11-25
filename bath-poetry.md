---
layout: default
title: bath poetry
---

<h1>bath poetry</h1>
<p>uhhhhhm think of something to say here...</p>

<ul class="poetry-list">
{% assign poetry_posts = site.posts | where:"categories","poetry" | sort:"date" | reverse %}
{% for post in poetry_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
    <p>{{ post.excerpt }}</p>
  </li>
{% endfor %}
</ul>
