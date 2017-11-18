---
layout: page
---
<h1>Blog post list</h1>
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><span> - {{post.date | date_to_long_string}}</span>
    </li>
  {% endfor %}
</ul>