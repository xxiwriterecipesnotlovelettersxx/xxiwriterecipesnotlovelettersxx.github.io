---
layout: default
title: recipes
---

<h1>recipes</h1>
<p></p>i looove cooking and sharing the food that i make! these are a lot of my favourite recipes and foods my friends told me they liked. my two most famous recipes are my <a href="/recipe/2025/11/25/vegan-cookies-that-i-brought-to-spit">cookies</a> and my <a href="/recipe/2025/11/25/spiced-morrocan-pumpkin-gay-vegan-woke-soup">soup</a>. but whatever... there's other cool stuff here too &lt;3

<ul class="recipe-list">
{% assign recipe_posts = site.posts | where:"categories","recipe" | sort:"date" | reverse %}
{% for post in recipe_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>
