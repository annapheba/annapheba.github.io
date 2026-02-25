
<div class="main-content">

<div class="hero">
  <h1>Hi, I'm Pheba 🌸</h1>
  <p>Welcome to my page, where I ramble on about anything I like. ✨</p>
  <a class="button" href="/about/">Get to Know Me</a>
</div>

<hr>

## 🚀 Latest Posts

{% for post in site.posts limit:5 %}
  <div class="post-card">
    <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
    <p>{{ post.excerpt }}</p>
  </div>
{% endfor %}

</div>
