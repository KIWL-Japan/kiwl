---
title: News
permalink: /news/
---

# News

{% if site.posts.size > 0 %}
  <div class="post-list">
    {% for post in site.posts %}
      <article class="post-card">
        <p class="post-date">{{ post.date | date: "%B %-d, %Y" }}</p>
        <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
        {% if post.excerpt %}
          {{ post.excerpt }}
        {% endif %}
      </article>
    {% endfor %}
  </div>
{% else %}
  <p>No news posts have been published yet.</p>
{% endif %}
