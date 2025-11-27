---
layout: default
title: Fragments
---

## 掲載記事

ここに掲載している記事は、プロジェクトメンバーによる
投稿をまとめたものです。

### 掲載年

<!-- 年ごとのリンク一覧 -->
<ul>
  {% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}
  {% for group in posts_by_year %}
    <li><a href="#year-{{ group.name }}">{{ group.name }}年</a></li>
  {% endfor %}
</ul>

<!-- 記事一覧（年ごとに分類） -->
{% for group in posts_by_year %}
  <h3 id="year-{{ group.name }}">{{ group.name }}年掲載記事</h3>
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

* [新潟LIVEカメラ](live-cam.html)
* [リンク集](link.html)

[back](./)
