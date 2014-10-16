---
layout: post
title: "Veure les estrelles. Jordi Mitjà, 2014"
share: true
class: artwork
class2: oferta
categories:
  - artwork
  - home
  - emocionart-analogic
  - jordi-mitja
published: true
work: 3310
---

{% assign work_data = site.data.works-emocionart-analogic | where:"id", page.work %}
{% assign work = work_data | first %}
<figure class="text-center">
	<div class="padding-artwork-container">
		<div class="embed-container embed-container_9-16">
			<core-image sizing="cover" class="core-image-size" preload fade src="{{ work.featured_src }}"></core-image>	
		</div>
	</div>
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{{ work.price_html }}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
<!--more-->
{% if work.description != null %}{{ work.description }}{% endif %}