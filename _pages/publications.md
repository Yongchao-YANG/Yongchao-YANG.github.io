---
title: "Publications - Dynamics & Intelligent Systems Group"
layout: gridlay
excerpt: "Publications -- Dynamics & Intelligent Systems Group."
sitemap: false
permalink: /publications/
---


# Publications

## Group highlights

(For a full list of publications and [patents](#Patents) see [below](#full-list-of-publications) or go to [Google Scholar](https://scholar.google.com/citations?user=gVH1w4kAAAAJ&hl=en), [ORCID](https://orcid.org/0000-0003-1776-3306). Some project updates are also at [Researchgate](https://www.researchgate.net/project/Full-field-Imaging-and-Modeling-of-Structural-Dynamics-by-Video-Motion-Manipulations).

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Patents
<!--<em>Milan P Allan, S Gröblacher, RA Norte, M Leeuwenhoek</em><br />Novel atomic force microscopy probes with phononic crystals<br /> PCT/NL20-20/050797 (2020)-->

<em>Yang, Y.</em> (2021)<br />Full-Field Imaging Learning Machines (FILM)<br /> US Patent Number: 11,127,127.
 
 <em>Yang, Y., Kenyon, G., Farrar, C., Mascarenas, D.</em> (2020)<br />System and method for automated extraction of high resolution structural dynamics from video<br /> <a href="https://patents.google.com/patent/US10567655B2/en">US Patent 10,567,655</a>.

<!--<em>Milan P Allan</em><br /> Methods of manufacturing superconductor and phononic elements <br /> <a href="https://patents.google.com/patent/US10439125B2/en?inventor=Milan+ALLAN&oq=inventor:(Milan+ALLAN)">US10439125B2 (2016)</a> -->

## Full List of publications
(go to [Google Scholar](https://scholar.google.com/citations?user=gVH1w4kAAAAJ&hl=en) for a complete list)
{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
