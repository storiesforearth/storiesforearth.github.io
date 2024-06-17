---
layout: page
title: Episodes
permalink: /category/episodes/
---

<ul>
  {% assign podcast_episodes = site.posts | where: "category", "episodes" %}
  {% if podcast_episodes.size > 0 %}
    {% for post in podcast_episodes %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span>{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  {% else %}
    <div>There's nothing to see here yet.</div>
  {% endif %}
</ul>