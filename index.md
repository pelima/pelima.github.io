<!-- index.html -->
---
layout: default
---

{% for post in site.posts %}
  <div class="post">
    <h2 class="post-title"><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-date">{{ post.date | date: "%B %e, %Y" }}</p>
    <div class="post-content">
      {{ post.content }}
    </div>
  </div>
{% endfor %}
