---
title: Events
permalink: /events/
---

# Events

{% if site.events.size > 0 %}
  <div class="post-list">
    {% for event in site.events %}
      <article class="post-card">
        <h2><a href="{{ event.url | relative_url }}">{{ event.title }}</a></h2>
        {% if event.excerpt %}
          {{ event.excerpt }}
        {% endif %}
      </article>
    {% endfor %}
  </div>
{% else %}
  <p>No events have been published yet.</p>
{% endif %}
