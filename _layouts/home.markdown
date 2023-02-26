---
layout: base
---

<div class="home">
    <div class="left-nav">
        <h2>Partners</h2>
        <ul>
          {% assign filtered_resources = site.publishers | where: 'type', 'Partner' %}
          {% for resource in filtered_resources %}
            <li><a href="{{ resource.url }}">{{ resource.name }}</a></li>
          {% endfor %}
        </ul>


        <h2>Community</h2>
        <ul>
          {% assign filtered_resources = site.publishers | where: 'type', 'Community' %}
          {% for resource in filtered_resources %}
            <li><a href="{{ resource.url }}">{{ resource.name }}</a></li>
          {% endfor %}
        </ul>
    </div>
    

  <div class="content">
    {{ content }}
  </div>
</div>