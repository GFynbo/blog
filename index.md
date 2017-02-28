---
layout: default
---

Recent posts
============
***

<ul>
  {% for post in site.posts %}
      <a href="/blog{{ post.url }}"><h2>{{ post.title }}</h2></a>
      <p style="padding-bottom: 50px;">{{ post.summary }}</p>
  {% endfor %}
</ul>
