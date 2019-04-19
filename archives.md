---
layout: page
<<<<<<< HEAD:archives.md
title: Archives
permalink: /archives/
=======
title: Blog Posts
permalink: /posts/
>>>>>>> 15992ea7de072f533989831723cff7ed20fd7c13:blogposts.md
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
