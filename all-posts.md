---
layout: page
title: All Posts
permalink: /all-posts/
published: true
---
Here's an index of all the posts I've ever written on this blog (most recent first):
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> {{ post.date | date: "%B %e, %Y" }}
    </li>
  {% endfor %}
</ul>
Enjoy!
