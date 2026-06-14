---
title: Home
layout: default
---

<section class="hero">
  <div class="hero-copy">
    <p class="eyebrow">Road cycling for charity in Japan</p>
    <h1>KIWL rides to support Mirai no Mori.</h1>
    <p class="hero-lede">Endurance rides, community events, and fundraising challenges that turn hard kilometers into support for children across Japan.</p>
    <div class="hero-actions">
      <a class="button" href="{{ "/about/" | relative_url }}">About KIWL</a>
      <a class="button button-secondary" href="{{ "/news/" | relative_url }}">Latest News</a>
    </div>
  </div>
</section>

<section class="feature-grid">
  <article>
    <img src="{{ "/assets/images/kiwl-coastal-ride-japan.png" | relative_url }}" alt="Road cyclists riding along a dramatic coastal road in Japan">
    <div>
      <p class="eyebrow">Ride</p>
      <h2>Big roads, bigger purpose</h2>
      <p>KIWL brings riders together for demanding road cycling events across Japan, raising awareness and funds for Mirai no Mori.</p>
    </div>
  </article>

  <article>
    <img src="{{ "/assets/images/kiwl-mountain-fundraising-japan.png" | relative_url }}" alt="Cyclists and road bikes at a mountain viewpoint in Japan after a charity ride">
    <div>
      <p class="eyebrow">Impact</p>
      <h2>Supporting outdoor programs</h2>
      <p>Funds raised by KIWL help Mirai no Mori create outdoor experiences where children build confidence, resilience, and connection.</p>
    </div>
  </article>
</section>

<section class="latest-news">
  <div class="section-heading">
    <p class="eyebrow">Updates</p>
    <h2>Latest News</h2>
  </div>
  <div class="post-list">
    {% for post in site.posts limit:3 %}
      <article class="post-card">
        <p class="post-date">{{ post.date | date: "%B %-d, %Y" }}</p>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        {{ post.excerpt }}
      </article>
    {% endfor %}
  </div>
</section>
