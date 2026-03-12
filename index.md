---
layout: default
title: Home
---

<section class="hero">
  <p class="hero-kicker">A journal where I ramble through the noise and the quiet moments in my head.</p>
  <h1>Hi, I'm Pheba <span class="anna-highlight">Anna</span> Philip 🌸</h1>
  <p class="hero-subtitle">I write about my life, memories, and the beauty of ordinary days.</p>
</section>

<section class="about-section">
  <p class="about-lead">Hi, there! Thank you for stopping by.</p>
  <p>This website is my space to talk about things that made me think twice, share a few things, and journal whatever comes to my mind. I was waiting for the perfect space to write, and then I realized I just needed to start somewhere, and here we are. Most of it might not make sense to you, but if it does, yaay. I am not entirely sure where I am going with this, but it is going to be me pouring my heart out with some human-generated content.</p>
  <p><a class="about-more-link" href="/about/">More about me ></a></p>
</section>

<section class="about-section">
  <h2>Latest posts</h2>
  <div class="write-grid">
    {% for post in site.posts limit: 1 %}
    <article class="write-card">
      <a class="write-card-link" href="{{ post.url | relative_url }}">
        <p class="hero-kicker">{{ post.date | date: "%d %B %Y" }}</p>
        <h3>{{ post.title }}</h3>
        {% if post.excerpt %}
        <p>{{ post.excerpt | strip_html | truncate: 140 }}</p>
        {% endif %}
        <span>Open -></span>
      </a>
    </article>
    {% endfor %}
  </div>
</section>

<section class="about-section">
  <h2>Contact</h2>
  <p>I would love to hear from you.</p>
  <p><strong>Email:</strong> <a href="mailto:phebaannaphilip@gmail.com">phebaannaphilip@gmail.com</a></p>
</section>
