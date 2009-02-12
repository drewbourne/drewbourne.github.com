---
layout: default
---

<section class="what">
  <article>
  {% for post in site.posts limit:1 %}
    <header>
      <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
    </header>
    <p class="meta">{{ post.date | date_to_string }}</p> 
    {{ post.content }}
  {% endfor %}
  </article>
</section>