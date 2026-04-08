---
title: Web
author: Dor0r0
date: 2026-04-08
category_key: web
layout: post
permalink: /categories/web/
---

`web` 카테고리입니다.

## 서브카테고리

- [CTF]({{ site.baseurl }}/categories/web/ctf/)

## 글 목록

{% assign category_posts = site.posts | where_exp: "post", "post.category == page.category_key or post.categories contains page.category_key" %}
{% assign direct_posts = category_posts | where_exp: "post", "post.subcategory == nil or post.subcategory == ''" %}

{% if direct_posts.size > 0 %}
{% for post in direct_posts %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}
{% else %}
아직 상위 카테고리에 직접 등록된 글이 없습니다.
{% endif %}
