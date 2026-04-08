---
layout: page
title: Archive
permalink: /archive/
description: "작성한 글 전체 목록"
---

{% if site.posts.size > 0 %}
<div class="archive-list">
  {% for post in site.posts %}
    <article class="archive-item">
      <p class="archive-date">{{ post.date | date: "%Y.%m.%d" }}</p>
      <h2 class="archive-title">
        <a href="{{ post.url | relative_url }}" class="text-decoration-none">{{ post.title }}</a>
      </h2>
      <p class="archive-excerpt mb-0">{{ post.excerpt | strip_html | strip | truncate: 180 }}</p>
    </article>
  {% endfor %}
</div>
{% else %}
<div class="empty-state">
  <p class="mb-0">아직 작성된 글이 없습니다.</p>
</div>
{% endif %}
