---
layout: page
title: Artworks
category: mur-diari
---
<h2>Digital</h2>
<div class="posts clearfix">
  {% for post in site.categories['emocionart-digital'] %}
  <div class="post">

    {{ post.excerpt }}    

  <h2 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <p class="text-center"><a href="{{ post.url }}"><i class="fa fa-lg fa-plus-square-o"></i></a></p>
    </div>
  {% endfor %}
</div>
---
<h2>Analógico</h2>
<div class="posts clearfix">
  {% for post in site.categories['emocionart-analogic'] %}
  <div class="post">

    {{ post.excerpt }}    

  <h2 class="post-title">
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </h2>
    <p class="text-center"><a href="{{ post.url }}"><i class="fa fa-lg fa-plus-square-o"></i></a></p>
    </div>
  {% endfor %}
</div>
