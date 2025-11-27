---
layout: default
title: shows
---

<h1>shows</h1>
<p class="recipe-intro">a page to document the shows i go to! a collection of photography, aaaaaaaaaaaaaaaa</p>

<br>
<ul class="shows-list">
{% assign show_posts = site.posts | where:"categories","show" | sort:"date" | reverse %}
{% for post in show_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>
