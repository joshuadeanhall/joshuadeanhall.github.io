---
layout: home
---

<h1>{{ page.name }}</h1>
<h2>{{ page.position }}</h2>

{{ content }}


<h2>Resources</h2>
<ul>
  {% assign filtered_resources = site.resources | where: 'publisher', page.name %}
  {% for resource in filtered_resources %}
    <li><a href="{{ resource.url }}">{{ resource.name }}</a></li>
  {% endfor %}
</ul>