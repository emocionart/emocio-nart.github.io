---
layout: post
title: "Caseta Magica a #emocionart"
og: true
og-type: article
share: true
class2: oferta
categories:
  - oferta
published: true
work: 2606
---

{% assign work_data = site.data.casetes %}
{% assign work = work_data %}
{% for work in work limit:1 %}
<figure class="text-center">
	<div class="padding-artwork-container">
		<a href="{{ page.url }}" title="{{ page.title }}">
			<div class="embed-container embed-container_3-4">
				<core-image sizing="cover" class="core-image-size" preload fade src="{{ work.featured_src }}"></core-image>	
			</div>
		</a>
	</div>
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{{ work.price_html }}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
{% endfor %}

<!--more-->

Aquesta setmana [Artinpocket](http://www.artinpocket.cat/) us vol presentar a [Caseta Mágica](http://www.artinpocket.cat/product-tag/caseta-magica/). Aquest projecte artístic neix a València i desenvolupa el seu treball dins el món gràfic. El procés creatiu i en conseqüència les seves peces són un reflex de la necessitat de transformar el que ens envolta, de revisió d'allò establert. Aquesta premissa la duen a terme donant marge a l'espontaneïtat, al joc i a la diversió. Caseta Magica entén "el treball com a creació i la vida com a treball creatiu".

Els  dos collages que us oferim de Caseta Mágica són Hilar el Cielo y No me Interrumpas. Aquestes dues  peces, amb títols tant poètics, són realitzades amb objectes trobats que ja existien prèviament. La nova utilització ens aporta un canvi de visió que actua com a generador de pensament, d'actitud i de percepció de la realitat; tot això s'aconsegueix donant valor a lo inútil. Dit d'altre manera aquestes treballs són pura poesia.

No me interrumpas y Hilar el cielo són dos collages de Caseta Mágica que trobareu dins [#emocionart](https://twitter.com/search?f=realtime&q=%23emocionart), art exclusiu i original accessible per a tothom. Entreu a [www.emocio-nart.com](/) i gaudiu de les nostres promocions.

{% assign work_data = site.data.casetes %}
{% assign work = work_data %}
{% for work in work offset:1 %}
<figure class="text-center">
	<div class="padding-artwork-container">
		<div class="embed-container embed-container_3-4">
			<core-image sizing="cover" class="core-image-size" preload fade src="{{ work.featured_src }}"></core-image>	
		</div>
	</div>
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{{ work.price_html }}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
{% endfor %}