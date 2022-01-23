---
  # _pages
  - scope:
      path: ""
      type: pages
    values:
      layout: single
#has_children: true
#has_toc: false
---

### 블로그

<ul class="posts">
   {% for post in site.posts %}
      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
   {% endfor %}
</ul>