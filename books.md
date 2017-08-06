---
layout: page
title: Books
permalink: /books/

---
I read loads of books. These are some I've made notes on.



<ul>
  {% for post in site.categories.BOOKS %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> {{ page.date | date: "%B %e, %Y" }}
    </li>
  {% endfor %}
</ul>
