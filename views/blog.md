---
layout: 'base.njk'
renderData: 
  title: 'Blog'
---

{# TODO: Reverse #}
{% for year, posts in posts | groupby("year") %}

## {{ year }}
  
{% for post in posts %}
* {{ post.date }} - [{{ post.title }}](/blog/{{ post.slug }})
{% endfor %}
{% endfor %}

[Blog Archiv](/blog/archive)
