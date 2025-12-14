---
layout: default
title: Home
---
# Home Page

[My First Blog Post]({{ site.baseurl }}{% post_url 2025-12-14-test-post %})

Here are my latest posts:

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
      <span> — {{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
