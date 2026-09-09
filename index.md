---
layout: home
title: Home
---

<h1 class="home-heading">Hi, I'm Fredrik</h1>
<p class="home-subtitle">D365FO developer · Azure integrations · Sweden</p>

<p class="home-bio">I'm a D365FO developer/consultant based in Sweden. I am spending my days elbow-deep in X++ and Azure integrations. This site is where I write up what I learn along the way.</p>

<div class="home-actions">
  <a class="btn" href="{{ '/blog/' | relative_url }}">Read the blog</a>
</div>

<hr class="home-divider">

<div class="home-section-header">
  <h2>Latest posts</h2>
  <a class="home-view-all" href="{{ '/blog/' | relative_url }}">View all</a>
</div>

<div class="post-cards">
  {%- for post in site.posts limit: 3 -%}
  <a class="post-card" href="{{ post.url | relative_url }}">
    <span class="post-card-date">{{ post.date | date: "%b %Y" }}</span>
    <h3 class="post-card-title">{{ post.title | escape }}</h3>
    <p class="post-card-excerpt">{{ post.excerpt | strip_html | truncate: 90 }}</p>
  </a>
  {%- endfor -%}
</div>
