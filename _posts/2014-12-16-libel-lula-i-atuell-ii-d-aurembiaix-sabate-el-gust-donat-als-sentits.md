---
layout: post
title: "Libèl.lula i atuell II. d'Aurembiaix Sabaté, el gust donat als sentits"
og: true
og-type: article
share: true
class2: oferta
categories:
  - oferta
published: true
work: 2660
---

{% assign sale_date = site.time | date_to_xmlschema %}
{% assign work_data = site.data.works-emocionart-analogic | where:"id", page.work %}
{% assign work = work_data | first %}
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
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{% if sale_date > site.sale-end %}{{ work.regular_price }}{% else if %}{{ work.price_html }}{% endif %}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
<!--more-->

Una peça d'art és l'expressió de la sensibilitat d'un artista. El diccionari defineix "regal" com *El gust donat als sentits* i "regalar" és definit com a *delitar, causar plaer*. La millor manera per fer-ho és regalar art, un regal memorable que marca la diferència. **[Libèl.lula i atuell II]({{ work.permalink }})**, d'Aurembiaix Sabaté és una bona opció per a transmetre la sensibilitat d'aquesta artista i complaure aquella persona que apreciem amb un obsequi únic i exclusiu.

Obra inspirada en Haikus del Llibre "Postals no escrites", de la Felícia Fuster.

>M'interessa el diàleg que tenim com a éssers humans amb el medi en l'àmbit cognitiu i espiritual. A través de l'observació de la natura, plasmar instants anecdòtics, juntament amb alguns objectes i símbols, indagant així en la percepció que existeix quan estem amb atenció, per això la presència dels elements es mostra tan contundent, emergint en el blanc, endinsant-nos en un procés de meditació i calma, a través de la contemplació i la maduració del que s'esdevé en el nostre entorn.