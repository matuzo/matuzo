---
layout: 'base.njk'
renderData: 
  title: 'Manuel Matuzovic'
---

## Recent blog posts

{% for post in posts %}
* {{ post.date }} - [{{ post.title }}](blog/{{ post.slug }})
  {{ post.body | safe }}
{% endfor %}
