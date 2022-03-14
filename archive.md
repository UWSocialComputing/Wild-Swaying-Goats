---
layout: page
title: Blog Archive
---

{% for tag in site.tags %}
  <ul>
    {% for post in tag[1] %}
      <li><a href="/Wild-Swaying-Goats{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
