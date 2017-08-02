---
layout: page
title: All Posts
permalink: /all-posts/
---
Here's an index of all the posts I've ever written on this blog:
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> {{ page.date | date: "%B %e, %Y" }}
    </li>
  {% endfor %}
</ul>
Enjoy!
