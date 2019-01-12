---
title: Allison Schenker
layout: default
---
<div class="row carousel-row bg-dark">
  {% for portfolio in site.portfolios %}
    <div class="col home-features">
      <h2><a href="{{portfolio.url}}">{{portfolio.title}}</a></h2>
      <a href="{{portfolio.url}}"><img src="{{portfolio.img_src}}" alt="{{ portfolio.img_alt }}"/></a>
    </div>
  {% endfor %}
</div>