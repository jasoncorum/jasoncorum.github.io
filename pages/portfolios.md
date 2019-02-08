---
title: Portfolios
layout: default
---
<div class="row">
  {% for portfolio in site.portfolios %}
      <div class="col-12 col-md-6 portfolio">
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