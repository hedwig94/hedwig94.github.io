---
layout: page
title: Health Facts
excerpt: "Facts about food and health."
modified: 2014-08-08T20:04:41.231140-04:00
image:
  feature: food3.jpg
---

<ul class="post-list">
{% for post in site.categories.health-facts %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>