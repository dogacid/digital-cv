---
title: Coding
layout: home
nav_order: 1
---

## Coding posts
{% for tag in site.tags %}
  {% if tag[0] == "coding" %}
    {% for post in tag[1] %}
#### {{ post.date | date_to_string }} - [{{ post.title }}]({{ site.base_url }}{{ post.url }})

    {% endfor %}
  {% endif %}
{% endfor %}