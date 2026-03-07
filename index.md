<section class="hero">
  <p class="hero-kicker">A journal of ideas and quiet moments</p>
  <h1>Hi, I'm Pheba Anna Philip 🌸</h1>
  <p class="hero-subtitle">I write about life, creativity, and the beauty of ordinary days.</p>
  <div class="hero-actions">
    <a class="button" href="/about/">Get to Know Me</a>
    <a class="button button-outline" href="#latest-posts">Read the Blog</a>
  </div>
</section>

<section class="highlights" aria-label="Highlights">
  <article class="highlight-item">
    <h3>About Me</h3>
    <p>A curious soul sharing stories, thoughts, and creative sparks.</p>
    <a href="/about/">Learn more →</a>
  </article>
  <article class="highlight-item">
    <h3>What I Write</h3>
    <p>Personal reflections, random ideas, and things I discover along the way.</p>
    <a href="#latest-posts">Browse posts →</a>
  </article>
  <article class="highlight-item">
    <h3>Stay Connected</h3>
    <p>Come back often for fresh posts and updates from my blogging journey.</p>
    <a href="/">Visit again →</a>
  </article>
</section>

<section id="latest-posts" class="latest-posts">
  <div class="section-heading">
    <h2>Latest Posts</h2>
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
