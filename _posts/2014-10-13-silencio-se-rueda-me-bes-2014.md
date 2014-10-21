---
layout: post
title: "SILENCIO, SE RUEDA!. ME BES, 2014"
og: true
og-type: product
share: true
class: artwork
categories:
  - artwork
  - home
  - emocionart-analogic
published: true
work: 2472
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