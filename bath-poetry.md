---
layout: default
title: bath poetry
---

<h1>bath poetry</h1>
<p>these poems are mostly incoherent because that is what steam seems to do to me. if you find meaning in them that is exciting! happy reading xx</p>
<br>
<ul class="poetry-list">
{% assign poetry_posts = site.posts | where:"categories","poetry" | sort:"date" | reverse %}
{% for post in poetry_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>
