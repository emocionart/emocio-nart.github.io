---
layout: post
title: "Txus Leal Tejada a #emocionart"
og: true
og-type: article
share: true
class2: oferta
categories:
  - oferta
published: true
work: 2496
---

{% assign work_data = site.data.leals %}
{% assign work = work_data %}
{% for work in work limit:1 %}
<figure class="text-center">
	<div class="padding-artwork-container">
		<div class="embed-container embed-container_4-3">
			<core-image sizing="cover" class="core-image-size" preload fade src="{{ work.featured_src }}"></core-image>	
		</div>
	</div>
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{{ work.price_html }}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
{% endfor %}

<!--more-->

¿Sabes que es #emocionart? Se trata de **una acción de [Artinpocket](http://www.artinpocket.cat/) para promocionar e impulsar la compra de arte**. Como cada semana y durante tres meses os queremos presentar la obra de uno de los artistas de la plataforma.

**[La madurez de la joven de la perla](http://www.artinpocket.cat/product/la-madurez-de-la-joven-de-la-perla-txus-leal-tejada-2014-500/)** es una obra del creador audiovisual [Txus Leal Tejada](http://www.artinpocket.cat/product-tag/txus-leal-tejada/). Esta fotografía forma parte de la serie *Benditas locuras* y está inspirada en el retrato de *La Joven de la Perla* (1665) de Johannes Vermeer, uno de sus referentes pictóricos. Para Txus Leal, el paso del tiempo, las sensaciones, las influencias pictóricas impregnan cada fotografía que realiza y que –gracias a las técnicas digitales- traspasan la línea de la realidad y nos transportan a un mundo onírico, subjetivo e íntimo que conecta con la fibra emocional. Captar “la mirada del otro”  es la finalidad de este creador.  Txus Leal afirma: “*muchas de las fotografías se han realizado en momentos de rabia, miedo o inmensa alegría*”, así pues las emociones son el motor de su creatividad.

Esta obra es sin duda una magnífica propuesta para sumergirte en la experiencia de comprar arte. [#emocionart](https://twitter.com/search?q=%23emocionart&src=typd&f=realtime) con Txus Leal Tejada. Visita [www.emocio-nart.com](/) y descubrirás nuestras [promociones](/ofertas/).

{% assign work_data = site.data.leals %}
{% assign work = work_data %}
{% for work in work offset:1 %}
<figure class="text-center">
	<div class="padding-artwork-container">
		<div class="embed-container embed-container_4-3">
			<core-image sizing="cover" class="core-image-size" preload fade src="{{ work.featured_src }}"></core-image>	
		</div>
	</div>
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{{ work.price_html }}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
{% endfor %}