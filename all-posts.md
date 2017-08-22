---
layout: page
title: All Posts
permalink: /all-posts/
published: true
---
Here's an index of all the posts I've ever written on this blog (most recent first). Alternatively, just search the whole site on DuckDuckGo.
<iframe src="https://duckduckgo.com/search.html?width=200&site=https://dcisbusy.github.io&prefill=Search DuckDuckGo" style="overflow:hidden;margin:0;padding:0;width:258px;height:40px;" frameborder="0"></iframe>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> {{ post.date | date: "%B %e, %Y" }} in <em>{{ post.categories }}</em>
    </li>
  {% endfor %}
</ul>
Enjoy!
