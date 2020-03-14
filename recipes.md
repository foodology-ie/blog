---
layout: default
---

<div class="recipes">
  <h1>Recipes</h1>

  <div class="masonry">
    {% for recipe in site.recipes %}
      <div class="brick">
        <a href="{{ recipe.url | absolute_url }}">
          <img src="{{ recipe.image | default: '/assets/images/recipes/fallback.gif' | absolute_url }}" />
          <h2>{{recipe.title}}</h2>
        </a>
      </div>
    {% endfor %}
  </div>
</div>
