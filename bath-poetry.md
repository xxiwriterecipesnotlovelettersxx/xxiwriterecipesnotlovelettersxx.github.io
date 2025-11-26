---
layout: default
title: bath poetry
---

<h1>bath poetry</h1>
<p>uhhhhhm think of something to say here...</p>
<br>
<ul class="poetry-list">
{% assign poetry_posts = site.posts | where:"categories","poetry" | sort:"date" | reverse %}
{% for post in poetry_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>
