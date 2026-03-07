---
layout: default
title: Home
---

<section class="hero">
  <p class="hero-kicker">A journal to ramble through the noise and quiet moments in my head</p>
  <h1>Hi, I'm Pheba Anna Philip 🌸</h1>
  <p class="hero-subtitle">I write about my life, and the beauty of ordinary days.</p>
</section>

<section class="highlights" aria-label="Highlights">
  <article class="highlight-item">
    <h3>About Me</h3>
    <p>I waited for the perfect space to write, then realized I just needed an honest one.</p>
    <a href="/about/">Learn more →</a>
  </article>
  <article class="highlight-item">
    <h3>What I Write</h3>
    <p>Personal reflections, random ideas, and things I discover along the way.</p>
    <a href="#latest-posts">Browse posts →</a>
  </article>
</section>

<section id="writes" class="latest-posts">
  <div class="section-heading">
    <h2>Writes</h2>
    <p>Fresh thoughts from the blog.</p>
  </div>

  <div class="post-list">
    {% for post in site.posts limit:6 %}
      <article class="post-row">
        <p class="post-date">{{ post.date | date: "%b %-d, %Y" }}</p>
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p>{{ post.excerpt | strip_html | truncate: 150 }}</p>
      </article>
    {% endfor %}
  </div>
</section>

<section id="clicks" class="topic-section">
  <div class="section-heading">
    <h2>Clicks</h2>
    <p>Moments captured one frame at a time.</p>
  </div>
</section>

<section id="reads" class="topic-section">
  <div class="section-heading">
    <h2>Reads</h2>
    <p>Books, essays, and pieces that stay with me.</p>
    <a href="/reads/">View reading list →</a>
  </div>
</section>

<section id="travels" class="topic-section">
  <div class="section-heading">
    <h2>Travels</h2>
    <p>Places, routes, and reflections from the road.</p>
  </div>
</section>
