---
layout: default
title: Top Page
---

<main>
  <div class="caption">
    <h3>POSTS</h3>
  </div>
  {% for post in site.posts %}
    <aside>
      <h3>
      <div class="post-items">
        <div class="month">{{ post.date | date: "%b"}}</div>
        <div class="date-year">{{ post.date | date: "%d, %y" }}</div>
        <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      </div>
      </h3>
    </aside>  
  {% endfor %}
</main>