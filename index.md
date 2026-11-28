---
title: Home
layout: default
---

<section class="hero">
  <div class="hero-copy">
    <p class="eyebrow">Road cycling for charity in Japan</p>
    <h1>Get Fit &amp; Give Back With KIWL</h1>
    <p class="hero-lede">Our main pursuit is cycling but we also participate in running and walking events to raise funds for the support and development of children living in institutional care in Japan. Join us for an epic 4-day 500km cycle ride, take part in month-long cycling and running challenges, or a sedate walk or jog around the Imperial Palace in Tokyo. Something for everyone of all ages and abilities to get fit and give back to kids less fortunate.</p>
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
      <p>KIWL brings riders of all ages &amp; abilities together for demanding multi-day road cycling events across Japan, raising funds and awareness for our chosen charity. Our next big ride is the KIWL Classic in Tohoku from May 26th-30th 2027, applications open in January 2027.</p>
    </div>
  </article>

  <article>
    <img src="{{ "/assets/images/kiwl-mountain-fundraising-japan.png" | relative_url }}" alt="Cyclists and road bikes at a mountain viewpoint in Japan after a charity ride">
    <div>
      <p class="eyebrow">Impact</p>
      <h2>Supporting kids in care</h2>
      <p>Funds raised by KIWL support our chosen charity, Mirai No Mori NPO who provide outdoor programs designed to build self-confidence, teamwork and instil personal values that will transform them into happy and successful young adults.</p>
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
