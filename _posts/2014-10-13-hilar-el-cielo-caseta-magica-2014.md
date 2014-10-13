---
layout: post
title: "Hilar el cielo. Caseta Mágica, 2014"
share: true
class: artwork
categories:
  - artwork
  - home
  - emocionart-analogic
published: true
work: 2588
---

{% assign work_data = site.data.works-emocionart-analogic | where:"id", page.work %}
{% assign work = work_data | first %}
<figure class="text-center">
	<img src="{{ work.featured_src }}">
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{{ work.price_html }}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
<!--more-->
{% if work.description != null %}{{ work.description }}{% endif %}