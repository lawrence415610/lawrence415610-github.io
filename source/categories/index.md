---
title: categories
date: 2023-09-03 22:06:03
---

---
title: Categories
layout: categories
---

<!-- Categories List -->
{% for category in site.categories %}
  <h2 id="{{ category[0] }}">{{ category[0] }}</h2>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ url_for(post.path) }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}