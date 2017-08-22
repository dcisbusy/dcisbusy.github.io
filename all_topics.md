---
layout: page
title: All Topics
published: true
permalink: /all-topics/
---
<h2>Categories</h2>

{% capture categories %}
  {% for category in site.categories %}
    {{ category[0] }}
  {% endfor %}
{% endcapture %}
{% assign sortedcategories = categories | sort %}

{% for category in sortedcategories %}
  <h3 id="{{ category }}">{{ category }}</h3>
  <ul>
  {% for post in site.categories[category] %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
  </ul>
{% endfor %}

<h2>Tags</h2>

{% capture tags %}
  {% for tag in site.tags %}
    {{ tag[0] }}
  {% endfor %}
{% endcapture %}
{% assign sortedtags = tags | split:' ' | sort %}

{% for tag in sortedtags %}
  <h3 id="{{ tag }}">{{ tag }}</h3>
  <ul>
  {% for post in site.tags[tag] %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
  </ul>
{% endfor %}
