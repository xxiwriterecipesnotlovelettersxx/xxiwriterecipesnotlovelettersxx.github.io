---
layout: default
title: shows
---

<h1>shows</h1>
<p class="recipe-intro">a page to document part of the scene through the shows i go to! a journalistic collection of photography, articles, posters, etc.</p>

<br>
<ul class="post-list">
{% assign show_posts = site.posts | where:"categories","show" | sort:"date" | reverse %}
{% for post in show_posts %}
  <li>
    {% if post.thumbnail %}
      <span class="post-thumb">
        <a href="{{ post.url }}">
          <img src="{{ post.thumbnail }}" alt="">
        </a>
      </span>
    {% endif %}

    <a href="{{ post.url }}">
      {{ post.title }} - {{ post.date | date: "%b %-d, %y" }}
    </a>
  </li>
{% endfor %}
</ul>
