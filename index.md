---
layout: default
title: AI Journal
---

# {{ page.title }}
Notes, reflections, and progress from my AI learning journey.

---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small> — {{ post.date | date: "%b %-d, %Y" }}</small><br>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>
