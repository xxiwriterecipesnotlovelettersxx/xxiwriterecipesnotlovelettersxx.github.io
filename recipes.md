---
layout: default
title: recipes
---

<h1>recipes</h1>
<p>uhhhhhm think of something to say [cookies](/2025/11/25/spiced-morrocan-pumpkin-gay-vegan-woke-soup/) here...</p>
<br>
<ul class="recipe-list">
{% assign recipe_posts = site.posts | where:"categories","recipe" | sort:"date" | reverse %}
{% for post in recipe_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>
