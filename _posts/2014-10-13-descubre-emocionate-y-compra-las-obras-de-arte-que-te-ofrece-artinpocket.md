---
layout: post
title: "Descubre, emociónate y compra las obras de arte que te ofrece Artinpocket"
share: true
class2: oferta
categories:
  - oferta
published: true
---

{% assign work_data = site.data.alones %}
{% assign work = work_data %}
{% for work in work limit:1 %}
<figure class="text-center">
	<img src="{{ work.featured_src }}">
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{{ work.price_html }}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
{% endfor %}

<!--more-->

[#Emocionart](/) es una acción de Artinpocket para promocionar e impulsar la compra de arte. Durante tres meses la plataforma impulsará diferentes acciones con el objetivo de acercar el arte e incentivar la compra obras originales a precios asequibles. Con esta acción se pretende romper falsos mítos: ¿el arte es caro? ¡No siempre! ¿El Arte es para una minoría? ¡Falso! 

Descubre y emociónate con el arte que te ofrece Artinpocket, obras de arte originales a precios asequibles para regalar o para decorar de forma personal tu casa. Por qué gastarse 100€ en una reproducción o comprar esas obras impersonales, fabricadas en cadena que encontramos en el Ikea pudiendo tener una obra original en casa. ¡Compra arte original!

Esta semana y de forma exclusiva os presentamos a  **Alona Vinç**, mujer que proviene del mar y que cambia de apellido como parte de una historia vital indisociable a las transformaciones que uno experimenta año tras año, relación tras relación, trabajo tras trabajo. Con ese consciente bagaje, tiene mucho que contar y lo narra con sus habilidades gráficas y, aunque ella no lo reconozca, también textuales.

**¡Sus obras de arte rebajadas un 15% y con transporte gratuito!** #Emocionart, arte económico al alcance de tu bolsillo con un solo clic.

{% assign work_data = site.data.alones %}
{% assign work = work_data %}
{% for work in work offset:1 %}
<figure class="text-center">
	<img src="{{ work.featured_src }}">
	<figcaption>
		<p><small><strong>{{ work.title }}</strong> | {% if work.downloadable == true %} digital art{% else if %} dimensiones: {{ work.dimensions.length }}x{{ work.dimensions.height }} {{ work.dimensions.unit }}{% endif %}</small></p>
		<p><a href="{{ work.permalink }}" class="btn btn-primary btn-lg">¡{{ work.price_html }}! ¡comprar! <i class="fa fa-credit-card"></i></a></p>
	</figcaption>
</figure>
{% endfor %}