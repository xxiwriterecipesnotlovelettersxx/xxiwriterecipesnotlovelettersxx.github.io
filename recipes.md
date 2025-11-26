---
layout: default
title: recipes
---

<h1>recipes</h1>
<p/>i looove cooking and sharing the food that i make! here i document a lot of my favourite recipes and the foods that other people have told me they like. my two most famous recipes are my
<a href="https://xxiwriterecipesnotlovelettersxx.github.io/recipe/2025/11/25/vegan-cookies-that-i-brought-to-spit.html">cookies</a> 
and my
<a href="https://xxiwriterecipesnotlovelettersxx.github.io/recipe/2025/11/25/spiced-morrocan-pumpkin-gay-vegan-woke-soup.html">soup</a>. 
but whatever... there's other cool stuff here too <3
</p>
<br>
<ul class="recipe-list">
{% assign recipe_posts = site.posts | where:"categories","recipe" | sort:"date" | reverse %}
{% for post in recipe_posts %}
  <li>
    <a href="{{ post.url }}">{{ post.title }} - {{ post.date | date: "%B %-d, %Y" }}</a>
  </li>
{% endfor %}
</ul>
