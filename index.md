---
layout: page
title: Light Digest
---
### Topics
<ul class="tag_box inline">
  {% assign tags_list = site.tags %}  
  {% include JB/tags_list %}
</ul>

### Latest
<ul class="posts">
  {% for post in site.posts limit:10 %}
  <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>