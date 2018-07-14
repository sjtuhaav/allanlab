---
title: "SJTUHAAV Lab - Pictures"
layout: piclay
excerpt: "SJTUHAAV Lab -- Pictures"
permalink: /pictures/
---


## Our video

#### Our uav 

<video width="480" height="320" controls>
<source src="{{ site.url }}{{ site.baseurl }}/images/video/nezha.mp4">
</video>


## Zeng Zheng
Group leader of SJTUHAAV in [SJTU](https://www.sjtu.edu.cn/).
<figure>
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/zengzheng.png" width="60%">
</figure>

#### Gallery
(Right-click *'view image'* to see a larger image.)
{% assign number_printed = 0 %}
{% for pic in site.data.pictures_Leiden %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-3 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/Gallery/{{ pic.image }}" class="img-responsive" width="95%" style="float: left" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>
