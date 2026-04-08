---
title: Web / CTF
author: Dor0r0
date: 2026-04-08
category_key: web
subcategory_key: ctf
layout: post
permalink: /categories/web/ctf/
---

`web > ctf` 글 목록입니다.

{% assign category_posts = site.posts | where_exp: "post", "post.category == page.category_key or post.categories contains page.category_key" %}
{% assign subcategory_posts = category_posts | where_exp: "post", "post.subcategory == page.subcategory_key" %}

{% if subcategory_posts.size > 0 %}
{% for post in subcategory_posts %}
- [{{ post.title }}]({{ site.baseurl }}{{ post.url }})
{% endfor %}
{% else %}
아직 등록된 글이 없습니다.
{% endif %}
