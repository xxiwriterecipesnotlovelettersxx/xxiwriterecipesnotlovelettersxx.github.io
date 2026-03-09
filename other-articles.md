---
layout: default
title: other articles
---

<h1>other articles</h1>
<p class="recipe-intro">yooo aha xoxo</p>

<br>
<ul class="post-list">
{% assign article_posts = site.posts | where:"categories","article" | sort:"date" | reverse %}
{% for post in article_posts %}
  <li>
    {% if post.thumbnail %}
      <span class="post-thumb">
        <a href="{{ post.url }}">
          <img src="{{ post.thumbnail }}" alt="">
        </a>
      </span>
    {% endif %}

    <a href="{{ post.url }}">
      {{ post.title }} - {{ post.date | date: "%d/%m/%y" }}
    </a>
  </li>
{% endfor %}
</ul>
