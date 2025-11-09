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

{% if page.tags %}
  <p class="tags">
    Tags:
    {% for tag in page.tags %}
      <a href="/tags/{{ tag | slugify }}/">{{ tag }}</a>
    {% endfor %}
  </p>
{% endif %}

<h2>その他色々</h2>

* [リンク集](link.html)
* [その他](other.html)

[back](./)
