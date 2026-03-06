---
layout: default
title: Sujoung Dev Notes
---

설정으로 요소를 부르치고, 글이 보이기 시작해요.
개발하며 부닥친 상황들을 부당업을 사용해서 정리합니다.

## Posts

{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}
