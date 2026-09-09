---
layout: home
title: Blog
permalink: /blog/
---

<h1 class="page-heading">Blog</h1>

<ul class="post-list">
  {%- for post in site.posts -%}
  <li>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
    </h3>
    {%- if post.image -%}
    <a class="post-list-thumb-link" href="{{ post.url | relative_url }}">
      <img class="post-list-thumb" src="{{ post.image | relative_url }}" alt="">
    </a>
    {%- endif -%}
    <p>{{ post.excerpt | strip_html | strip }}</p>
  </li>
  {%- endfor -%}
</ul>
