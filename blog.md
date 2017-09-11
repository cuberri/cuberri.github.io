---
layout: index
---

<ul class="posts">
  {% for mypost in site.myposts %}
  <li>
    <small class="datetime muted" data-time="{{ mypost.date }}">{{ mypost.date | date_to_string }} </small>
    <a href="{{ mypost.url }}">
      {{ mypost.title }}<br />
    </a>
  </li>
  {% endfor %}
</ul>
