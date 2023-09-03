---
title: tags
date: 2023-09-03 22:05:51
---


<!-- Tags Cloud -->
<div class="tags-cloud">
{% for tag in site.tags %}
  <a href="{{ url_for(tag.path) }}" class="tag-link">
    {{ tag.name }} <span class="tag-count">{{ tag.posts.length }}</span>
  </a>
{% endfor %}
</div>