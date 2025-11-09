---
layout: default
title: Fragments
---

<h2>記事一覧</h2>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%Y年%m月%d日" }}</small>
    </li>
  {% endfor %}
</ul>

[back](./)
