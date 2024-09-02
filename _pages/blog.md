---
layout: default
title: posts
permalink: /posts/
---
# {{page.title}}

{% assign sorted_posts = site.posts | sort: 'title' | reverse %}

<ul>
{% for post in sorted_posts %}
  <li> <a href="{{ post.url }}">{{ post.title | downcase}}</a> - {{ post.date | date_to_long_string | downcase }} </li>
{% endfor %}
</ul>
