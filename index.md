---
title: Allison Schenker
layout: default
---
<div class="row carousel-row">
  <div id="carouselExampleFade" class="carousel slide carousel-fade col-12" data-ride="carousel">
    <div class="carousel-inner">
      {% assign images = site.images | where:'featured_home', true | sort: 'home_order' %}
      {% for image in images %}
        {% if forloop.first == true %}
          <div class="carousel-item active">
            <a href="/pages/portfolios"><img class="d-block w-100 carousel-img" src="{{image.img_src}}" alt="{{image.title}}"></a>
          </div>
        {% else %}
          <div class="carousel-item carousel-img">
            <a href="/pages/portfolios"><img class="d-block w-100" src="{{image.img_src}}" alt="{{image.title}}"></a>
          </div>
        {% endif %}
      {% endfor %}
    </div>
    <a class="carousel-control-prev" href="#carouselExampleFade" role="button" data-slide="prev">
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="sr-only">Previous</span>
    </a>
    <a class="carousel-control-next" href="#carouselExampleFade" role="button" data-slide="next">
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="sr-only">Next</span>
    </a>
  </div>
</div>
