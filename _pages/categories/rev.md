---
title: Rev
author: Dor0r0
date: 2026-04-08
category_key: rev
layout: post
permalink: /categories/rev/
---

`rev` 카테고리 글 목록입니다.

{% assign category_posts = site.posts | where_exp: "post", "post.category == page.category_key or post.categories contains page.category_key" %}

{% if category_posts.size > 0 %}
{% for post in category_posts %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}
{% else %}
아직 등록된 글이 없습니다.
{% endif %}
