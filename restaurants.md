---
layout: default
---

<h1>Restaurants</h1>
<div style="position: relative;">
{% for restaurant in site.restaurants %}
    <div class="cell">
        <a href="{{ restaurant.url | absolute_url }}">
            {{ restaurant.excerpt }}
            <h2>{{restaurant.title}}</h2>
        </a>
    </div>
{% endfor %}
</div>
