---
title: Home
---

# KIWL

KIWL is a charity group raising funds for Mirai no Mori, an organization that creates life-changing outdoor programs for children in Japan.

We bring people together through community events, endurance challenges, and fundraising campaigns that support young people as they build confidence, resilience, and new possibilities.

[Learn about KIWL]({{ "/about/" | relative_url }}){: .button }
[Read the latest news]({{ "/news/" | relative_url }}){: .button .button-secondary }

## Supporting Mirai no Mori

Mirai no Mori provides outdoor experiences for children who may not otherwise have access to them. KIWL fundraises to help make those programs possible.

## Latest News

{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url | relative_url }})  
  <span class="post-date">{{ post.date | date: "%B %-d, %Y" }}</span>
{% endfor %}
