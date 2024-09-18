---
layout: default
---

<div class="jumbotron">
  <h1 class="display-4">Hello, world!</h1>
  <p class="lead">Welcome to My Awesome Blog. Explore a variety of topics and stay updated with the latest posts.</p>
  <hr class="my-4">
  <p>Discover articles on technology, tutorials, tips, and much more.</p>
  <a class="btn btn-primary btn-lg" href="#posts" role="button">Explore Posts</a>
</div>

<h2 id="posts">Latest Posts</h2>
<div class="list-group">
  {% for post in site.posts %}
    <a href="{{ post.url }}" class="list-group-item list-group-item-action">
      <h5 class="mb-1">{{ post.title }}</h5>
      <small>{{ post.date | date: "%B %d, %Y" }}</small>
      <p class="mb-1">{{ post.excerpt }}</p>
    </a>
  {% endfor %}
</div>
