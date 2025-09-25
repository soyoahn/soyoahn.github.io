---
layout: page
title: Blog
---

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}<br>{{ post.date | date: "%a %b %d, '%y" }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}