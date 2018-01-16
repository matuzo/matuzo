---
layout: 'base.njk'
renderData: 
  title: 'Blog Archive'
permalink: 'blog/archive'
---

{# TODO: Reverse #}
{% for year, postsarchive in postsarchive | groupby("year") %}

## {{ year }}
  
{% for post in postsarchive %}
* {{ post.date }} - [{{ post.title }}](/blog/{{ post.slug }})
{% endfor %}
{% endfor %}
