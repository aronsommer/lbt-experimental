---
title: Blog
has_children: false
nav_order: 9
has_toc: false
---

# Mein Blog

Hier ist mein Blog :)
{: .fs-6 .fw-300 }

{% for post in site.posts %}
  <article>
    <h2>
      <!-- <a href="{{ post.url }}"> -->
      <a href="/lbt-experimental{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <!-- <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> -->
    {{ post.content }}
  </article>
{% endfor %}
