---
layout: 'base.njk'
renderData: 
  title: 'Speaking'
---

{# TODO: Reverse #}
{% for year, talks in talks | groupby("year") %}

## {{ year }}
  
{% for talk in talks %}
* {{ talk.date }} - {{ talk.title }} at [{{ talk.event.title }}]({{ talk.event.url }})
  {% if talk.slides %}
  [Slides <span class="visually-hidden">for {{ talk.title }}</span>]({{ talk.slides }})
  {% endif %}
{% endfor %}
{% endfor %}
