---
layout: page
title: Episodes
permalink: /category/episodes/
---
Follow along as we discuss books, movies, TV shows, and more to explore what certain themes and characters can teach us about responding to climate change.
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