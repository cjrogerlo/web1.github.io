---
layout: page
title: Blog Posts
---
<p>Here are my blog posts and articles. Enjoy.</p>

<div>
{% assign posts_list = site.posts %}
{% for node in posts_list %}
  {% if node.title != null %}
    {% if node.layout == "post" %}
      <a class="page{% if post.url == node.url %} active{% endif %}" href="{{ node.url }}">{{ node.title }}</a>
      <br>
    {% endif %}
  {% endif %}
{% endfor %}
</div>
