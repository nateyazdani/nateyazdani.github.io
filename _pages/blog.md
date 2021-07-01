---
layout: default
permalink: /blog/
title: research blog
description: My thoughts about research
navigation: blog
---

<div class="header-bar">
  <h1>{{ site.blog_name }}</h1>
  <h2>{{ site.blog_description }}</h2>
</div>


<ul class="post-list">
  {% for post in paginator.posts %}
    <li>
      <h2 class="post-title"><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h2>
      <p class="post-meta">{{ post.date | date: '%B %-d, %Y — %H:%M' }}</p>
      <p class="post-description">{{ post.description }}</p>
    </li>
  {% endfor %}
</ul>

{% include pagination.html %}
