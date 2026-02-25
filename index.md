
<div class="hero">
  <h1>Hi, I'm Pheba 👋</h1>
  <p>Product Manager • Rambler • Dreamer</p>
  <a class="button" href="/about/">About Me</a>
</div>

<hr>

## 🚀 Latest Posts

{% for post in site.posts limit:3 %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.excerpt }}</p>
{% endfor %}
