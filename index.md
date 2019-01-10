---
title: Allison Schenker
layout: default
---
<h1>Portfolios</h1>
<div class="row">
  {% for portfolio in site.portfolios %}
    <div class="col-md-6">
      <div class="card mb-4 box-shadow">
        <img class="card-img-top" src="{{portfolio.img_src}}" alt="{{ portfolio.img_alt }}">
        <div class="card-body">
          <a href="{{portfolio.url}}" type="button" class="btn btn-sm btn-outline-secondary">View</a>
          <h3>{{portfolio.title}}</h3>
        </div>
      </div>
    </div>
  {% endfor %}
</div>