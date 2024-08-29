---
#
# By default, content added below the "---" mark will appear in the home page
# between the top bar and the list of recent posts.
# To change the home page layout, edit the _layouts/home.html file.
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: page
title : Thots
---


This is where I share all my thoughts either in 2 lines or a blog format


{% for post in site.categories.thots %}
  <article>
    <h4>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span style="font-size: 0.6em; color: #888;">  {{ post.date | date: "%B %d, %Y" }}</span>
    </h4>
  </article>
{% endfor %}
