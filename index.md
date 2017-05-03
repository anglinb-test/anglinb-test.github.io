---
layout: default
title: My Home Page
---

<div class="hfeed">
  
  {% for post in site.posts %}
    <article class="hentry entry">
      <h1 class="entry-title">
        {{ post.title }}
      </h1>
      {{ post.content }}
      <p>Posted on <time class="published" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date }}</time></p>
    </article>
  {% endfor %}
  
</div>
