---
layout: default
---

<ul>
  {% for post in site.posts %}
      <a href="/blog{{ post.url }}"><h1>{{ post.title }}</h1></a>
      <p style="padding-bottom: 50px;">{{ post.summary }}</p>
  {% endfor %}
</ul>
