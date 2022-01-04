---
title: "Pictures - Dynamics & Intelligent Systems Group"
layout: piclay
excerpt: "Pictures -- Dynamics & Intelligent Systems Group"
permalink: /pictures/
---

# Pictures
<!--Jump to: [Michigan Tech](#michigan-tech), [Argonne](#argonne), [Los Alamos](#los-alamos), [Rice](#rice)-->


<!--## Michigan Tech -->

<!--#### Timelapse of our STM assembling [(see LION news item)](https://www.physics.leidenuniv.nl/index.php?id=11573&news=867&type=lion&ln=EN):
<iframe width="560" height="315" src="https://www.youtube.com/embed/3iKvUMv1h5A" frameborder="0" allowfullscreen></iframe> -->

#### Gallery & Lab
<!--(Right-click *'view image'* to see a larger image.)-->
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_misc %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-md-4 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

<!--{% if even_odd == 3 %}
</div>
{% endif %} -->

<p> &nbsp; </p>

<!--First advertisement.
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageLeiden_red.jpg" width="60%" >
</figure> -->


<!--## Argonne-->
<!--From the [group of Andreas Wallraff](http://www.qudev.ethz.ch/).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageETH_red.jpg" width="60%">
</figure> -->

<!--## Los Alamos-->
<!--From the [group of Seamus JC Davis](http://davisgroup.lassp.cornell.edu).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageCornell_red.jpg" width="60%">
</figure> -->

<!--## Rice-->
<!--From the [group of Felix Baumberger](http://dqmp.unige.ch/baumberger/) (now at University of Geneva).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/WebpageSTA_red.jpg" width="60%">
</figure> -->
