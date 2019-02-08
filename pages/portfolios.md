---
title: Portfolios
layout: default
---
<div class="row">
  {% for portfolio in site.portfolios %}
      <div class="col">
        <a href="{{portfolio.url}}">
          <div class="hovereffect">
            <img class="img-responsive portfolio-img" src="{{portfolio.img_src}}" alt="">
            <div class="overlay">
              <h2>{{portfolio.title}}</h2>
            </div>
          </div>
        </a>
      </div>
  {% endfor %}
</div>