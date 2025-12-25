---
layout: default
title: Home
---

# Welcome

I'm a software engineer passionate about building elegant solutions to complex problems.

## Recent Posts

<ul class="post-list">
{% for post in site.posts limit:5 %}
  <li class="post-list-item">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
    {% if post.excerpt %}
    <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
    {% endif %}
  </li>
{% endfor %}
</ul>

{% if site.posts.size == 0 %}
<p>No posts yet. Check back soon!</p>
{% elsif site.posts.size > 5 %}
<p><a href="{{ '/blog' | relative_url }}">View all posts →</a></p>
{% endif %}
