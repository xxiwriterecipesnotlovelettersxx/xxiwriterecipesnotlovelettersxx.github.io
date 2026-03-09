---
layout: default
title: more skramz journalism
---

<h1>more skramz journalism</h1>
<p>these poems are mostly incoherent because that is what steam seems to do to me. if you find meaning in them that is exciting! happy reading xx</p>
<br>
<ul class="article-list">
{% assign article_posts = site.posts | where:"categories","article" | sort:"date" | reverse %}
{% for post in poetry_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%d/%m/%y" }}</a>
  </li>
{% endfor %}
</ul>
