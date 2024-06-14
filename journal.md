---
layout: default
title: journal
permalink: /journal/
---
# {{page.title}}

{% assign sorted_posts = site.posts | sort: 'title' | reverse %}

<ul>
{% for post in sorted_posts %}
  <li> <a href="{{ post.url }}">{{ post.date | date_to_long_string | downcase}}</a> - {{ post.title }} </li>
{% endfor %}
</ul>