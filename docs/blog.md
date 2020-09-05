---
layout: default
title: 블로그
date: 
permalink: /posts/
nav_order: 8
#has_children: true
#has_toc: false
---

### 블로그

<ul class="posts">
   {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
   {% endfor %}
</ul>