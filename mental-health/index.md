---
layout: page
title: Mental Health
excerpt: "How to make the most out of your life."
search_omit: true
image:
  feature: food4.jpg
---

<ul class="post-list">
{% for post in site.categories.mental-health %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
