---
layout: default
title: Rapports
---
<ul class="posts">
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">
      <strong>{{ post.date | date: "%d/%m/%Y" }}</strong>
      · <span class="badge {{ post.type }}">{{ post.type | capitalize }}</span>
      · {{ post.title }}
    </a>
  </li>
{% endfor %}
</ul>
{% if site.posts.size == 0 %}
  <p class="muted">Aucun rapport publié pour l'instant.</p>
{% endif %}
