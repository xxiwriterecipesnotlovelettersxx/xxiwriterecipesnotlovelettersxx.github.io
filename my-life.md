---
layout: default
title: my life
---

<h1>my life</h1>
<p>uhhhhhm think of something to say here...</p>
<br>
<ul class="life-list">
{% assign life_posts = site.posts | where:"categories","life" | sort:"date" | reverse %}
{% for post in life_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>
