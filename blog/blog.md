---
title: Blog
has_children: true
nav_order: 9
has_toc: false
---

# Mein Blog

Hier ist mein Blog :)
{: .fs-6 .fw-300 }

Hier werden Links zu meinen Posts angezeigt:

<ul>
  {% for post in site.posts %}
    <li>
      <!-- <a href="{{ post.url }}">{{ post.title }}</a> -->
      <a href="/lbt-experimental{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

Hier werden alle Posts vollständig angezeigt:

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
