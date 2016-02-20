---
layout: page
title: Stories
permalink: /stories/
---

This is a page for really cool stories.

<ul class="post-list">
  {% for post in site.tags.story %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        <span class="post-excerpt">{{ post.excerpt }}</span>
      </h2>
    </li>
  {% endfor %}
</ul>
