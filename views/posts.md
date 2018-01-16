---
layout: base.njk
pagination:
  data: posts
  size: 1
  alias: post
permalink: blog/{{ post.slug }}/index.html
renderData: 
  title: '{{ post.title }}'
---

{{ post.teaser }}
{{ post.body }}
