---
layout: default
title: more skramz journalism
---

<h1>other articles</h1>
<p>yoooooooooooooo aha xoxo</p>
<br>
<ul class="article-list">
{% assign article_posts = site.posts | where:"categories","article" | sort:"date" | reverse %}
{% for post in poetry_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%d/%m/%y" }}</a>
  </li>
{% endfor %}
</ul>
