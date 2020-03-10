---
layout: default
---

<div class="grid" data-masonry='{ "itemSelector": ".cell", "fitWidth": true, "gutter": 10 }'>
    <h1>Recipes</h1>
    <div style="position: relative;">
    {% for recipe in site.recipes %}
        <div class="cell">
            <a href="{{ recipe.url | absolute_url }}">
                {{ recipe.excerpt }}
                <h2>{{recipe.title}}</h2>
            </a>
        </div>
    {% endfor %}
    </div>
</div>
