---
layout: page
title: New? Start here
permalink: /start-here/
---
Welcome to Stories for Earth, a climate change podcast about stories that can give us strength and resilience in fighting the climate crisis. However you stumbled upon the podcast, we’re glad you found us, and we hope that what we talk about on the show and write about on the blog will help you.

If you’re new to what we’re doing here, start with the episodes and articles below to learn more about what we’re up to. For the story of how we started, read [this letter](/about/#story) from our founder, Forrest Brown.
## Begin with these articles and episodes
<ul>
  {% assign start_here = site.posts | where: "tag", "start-here" %}
  {% if start_here.size > 0 %}
    {% for post in start_here %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span>{{ post.date | date: "%B %d, %Y" }}</span>
      </li>
    {% endfor %}
  {% else %}
    <div>There's nothing to see here yet.</div>
  {% endif %}
</ul>
---
_This page is a work in progress. Check back soon for more information, or feel free to [reach out](/about/#contact-us) if you have a specific question._