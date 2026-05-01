---
layout: page
title: Blog
permalink: /blog/
---

# Technical Blog

Learning in public. Every post is something I actually built, tested, or studied.

{% for post in site.posts %}
  <article>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }} • {{ post.categories | join: ', ' }}</p>
    <p>{{ post.excerpt }}</p>
  </article>
{% endfor %}
