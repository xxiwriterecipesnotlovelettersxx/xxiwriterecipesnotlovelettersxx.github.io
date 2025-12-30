---
layout: default
title: my life
---

<h1>my life</h1>
<p>hi OMG welcome to my life... what have i been up to lately?</p>

<ul class="post-list">
{% assign life_posts = site.posts | where:"categories","life" | sort:"date" | reverse %}
{% for post in life_posts %}
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
