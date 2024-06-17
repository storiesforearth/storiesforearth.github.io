---
layout: page
title: Blog
permalink: /category/blog/
---

<ul>
  {% assign blog_posts = site.posts | where: "category", "blog" %}
  {% if blog_posts.size > 0 %}
    {% for post in blog_posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span>{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  {% else %}
    <div>There's nothing to see here yet.</div>
  {% endif %}
</ul>