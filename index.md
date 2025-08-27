---
title: Home
layout: page
---

# Welcome
Hi, 


<ul>
  {% for post in site.posts limit:5 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>({{ post.date | date: "%b %-d, %Y" }})</small>
    </li>
  {% endfor %}
</ul>

<p><a href="/archive">View all posts →</a></p>