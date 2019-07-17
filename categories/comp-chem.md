---
layout: page
permalink: /blog/categories/comp-chem
---

<h3> Posts by Category : {{ page.title }} </h3>

<div class="card">
{% for post in site.categories.comp-chem %}
 <li class="category-posts"><span>{{ post.date | date_to_string }}</span> &nbsp; <a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</div>
