---
layout: page
title: Blog
excerpt: "An archive of blog posts sorted by date."
search_omit: true
image:
  feature: blogimg.jpg
  credit: Till Boverman
  creditlink: http://wegraphics.net/downloads/free-ultimate-blurred-background-pack/

---

<ul class="post-list">
{% for post in site.categories.blog %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>
