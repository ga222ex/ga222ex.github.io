---
layout: page
---
Blog post list
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a><span> - {{post.date | date_to_long_string}}</span>
    </li>
  {% endfor %}
</ul>

Blog posts by category

asd