<article class="posts">
  {% for post in site.posts %}
    <div class="post">
      <a href="{{ post.link }}">
        <div class="thumb">
          <img src="{{ post.img }}">
        </div>
        <header class="content">
          {{ post.title }}
          <p><span class="source">{{ post.source }}</span> {{ post.text }}</p>
        </header>
        <footer>
        </footer>
      </a>
    </div>
  {% endfor %}
</article>
