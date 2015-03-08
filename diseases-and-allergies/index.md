---
layout: page
title: Diseases and Allergies
excerpt: "You can find information about diseases and allergies here."
search_omit: true
image:
  feature: food5.jpg
---

<ul class="post-list">
{% for post in site.categories.diseases-and-allergies %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
