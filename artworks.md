---
layout: page
title: Selección de emocion(art)es
category: mur-diari
---

<h2 class="tooltip-description">Arte <abbr href="#" data-toggle="tooltip" title="{{ site.tooltip-analogic }}">Analógico</abbr></h2>
<div class="posts clearfix">
  {% for post in site.categories['emocionart-analogic'] reversed %}
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
<h2 class="tooltip-description">Arte <abbr href="#" data-toggle="tooltip" title="{{ site.tooltip-digital }}">Digital</abbr></h2>
<div class="posts clearfix">
  {% for post in site.categories['emocionart-digital'] reversed %}
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