---
layout: post
title: "Cercle Libèl·lula II. Aurembiaix, 2014"
og: true
og-type: product
share: true
class: artwork
categories:
  - artwork
  - home
  - emocionart-digital
published: true
work: 2112
---

{% assign sale_date = site.time | date_to_xmlschema %}
{% assign work_data = site.data.works-emocionart-digital | where:"id", page.work %}
{% assign work = work_data | first %}
<figure class="text-center">
	<div class="padding-artwork-container">
		<a href="{{ page.url }}" title="{{ page.title }}">
			<div class="embed-container embed-container_4-4">
				<core-image sizing="cover" class="core-image-size" preload fade src="{{ work.featured_src }}"></core-image>	
			</div>
		</a>
	</div>
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{% if sale_date > site.sale-end %}{{ work.regular_price }}{% else if %}{{ work.price_html }}{% endif %}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
<!--more-->
{% if work.short_description != null %}<blockquote class="blockquote-reverse">{{ work.short_description }}</blockquote>{% endif %}
{% if work.description != null %}{{ work.description }}{% endif %}