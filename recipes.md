---
layout: default
title: recipes
---

## recipes

{% for post in site.categories.recipe %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
