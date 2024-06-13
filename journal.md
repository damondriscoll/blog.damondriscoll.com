---
layout: default
title: journal
permalink: /journal
---
# {{page.title}}
<ol>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.date | date_to_long_string | downcase}}</a>
    </li>
  {% endfor %}
</ol>

