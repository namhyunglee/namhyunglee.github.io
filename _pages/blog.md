---
  # _posts
  - scope:
      path: ""
      type: pages
	nav_order: 2
	has_children: true
	has_toc: false
    values:
      layout: single
	title: 블로그
	date: 2018-03-23T04:02:42+09:00
---

### 블로그

<ul class="posts">
   {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
   {% endfor %}
</ul>