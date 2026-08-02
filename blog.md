---
layout: default
title: Writing
permalink: /blog/
---

# writing

<aside class="note">also available as an <a href="{{ '/feed.xml' | relative_url }}">rss feed</a></aside>

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%b %-d, %Y" }}</time>
    </li>
  {% endfor %}
</ul>
