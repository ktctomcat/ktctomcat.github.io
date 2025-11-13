---
layout: default
title: Fragments
---

## 記事一覧

### 各年へ

<!-- 年ごとのリンク一覧 -->
<ul>
  {% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}
  {% for group in posts_by_year %}
    <li><a href="#year-{{ group.name }}">{{ group.name }}年の記事</a></li>
  {% endfor %}
</ul>

<!-- 記事一覧（年ごとに分類） -->
{% for group in posts_by_year %}
  <h3 id="year-{{ group.name }}">{{ group.name }}年の記事</h3>
  <ul>
    {% for post in group.items %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small>{{ post.date | date: "%Y年%m月%d日" }}</small>
      </li>
    {% endfor %}
  </ul>
{% endfor %}

## 資料

* [リンク集](link.html)
* [その他](other.html)

[back](./)
