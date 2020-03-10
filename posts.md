---
layout: default
---

<h1>Posts</h1>
<div style="position: relative;">
{% for post in site.posts %}
    <div class="cell">
        <a href="{{ post.url | absolute_url }}">
            <h2>{{post.title}}</h2>
            {{ post.excerpt }}
        </a>
    </div>
{% endfor %}
</div>
