---
layout: 'base.njk'
pagination:
  data: pages
  size: 1
  alias: page
permalink: /{{ page.slug }}/index.html
renderData: 
  title: '{{ page.title }}'
---

{{ page.text }}
