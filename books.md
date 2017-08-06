---
layout: page
title: Books
permalink: /books/

---
I read loads of books. These are some I've made notes on.



<ul>
  {% for page in site.pages %}
    
      {% for books in page.categories %}
       
          <li><a href="{{ page.url }}">{{ page.title }}</a></li>
        
      {% endfor %}  <!-- page-category -->
   
  {% endfor %}  <!-- page -->
</ul>


<ul>
  {% for page in site.categories.BOOKS %}
    <li>
      <a href="{{ page.url }}">{{ page.title }}</a> {{ page.date | date: "%B %e, %Y" }}
    </li>
  {% endfor %}
</ul>


