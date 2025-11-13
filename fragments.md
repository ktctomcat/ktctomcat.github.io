---
layout: default
title: Fragments
---

<!-- 年ごとのリンク一覧 -->
<ul>
  {% assign years = "" | split: "" %}
  {% for post in site.posts %}
    {% assign year = post.date | date: "%Y" %}
    {% unless years contains year %}
      {% assign years = years | push: year %}
    {% endunless %}
  {% endfor %}
  {% assign years = years | sort | reverse %}
  {% for year in years %}
    <li><a href="#year-{{ year }}">{{ year }}年の投稿</a></li>
  {% endfor %}
</ul>

<!-- 投稿一覧（年ごとに分類） -->
{% for year in years %}
  <h2 id="year-{{ year }}">{{ year }}年の投稿</h2>
  <ul>
    {% for post in site.posts %}
      {% if post.date | date: "%Y" == year %}
        <li>
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          <small>{{ post.date | date: "%Y年%m月%d日" }}</small>
        </li>
      {% endif %}
    {% endfor %}
  </ul>
{% endfor %}

## 記事一覧

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%Y年%m月%d日" }}</small>
    </li>
  {% endfor %}
</ul>

## 資料

* [リンク集](link.html)
* [その他](other.html)

[back](./)
