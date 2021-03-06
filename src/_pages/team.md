---
layout: hero
title: "Equipe"
image:
  feature: banner-rotulo.png
permalink: /equipe/
---

<div class="row align-items-center pt-2">
    <div class="col-md-7">
        <h2>Equipe</h2>
        <hr class="pb-4">
        <p class="lead">O PRACTICE conta com uma equipe de estudantes e servidores que se dedicam de forma organizada e eficiente para realizar diversos tipos de atividades.</p>
    </div>
    <div class="col-md-1"></div>
    <div class="col-md-3 mt-4">
        <p><img alt="image" class="img-fluid" src="/images/icons/noun_team_2717434.svg"></p>
    </div>
</div>

<section class="fdb-block">
  <div class="container">
    <section class="pt-5">
      <h2 class="pb-3">Coordenação</h2>
      <hr class="pb-4">
      <h3>Coordenação Geral</h3>
      <div class="card-group">
        {% assign people = site.data.people | where:"position","coor-geral" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
      <h3>Coordenação Técnica-pedagógica</h3>
      <div class="card-group">
        {% assign people = site.data.people | where:"position","coor-tec" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
      <h3>Equipe Técnica Pedagógica Campus Laranjeiras do Sul</h3>
      <div class="card-group">
        {% assign people = site.data.people | where:"position","coor-tec-ls" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
    <section class="pt-5">
      <h2 class="pb-3">Produção de conteúdo</h2>
      <hr class="pb-4">
      <h3>Texto e imagem</h3>
      <div class="card-group">
        {% assign people = site.data.people | where:"position","con-material" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
      <h3>Imagem, vídeo e som</h3>
      <div class="card-group">
        {% assign people = site.data.people | where:"position","con-midia" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
    <section class="pt-5">
      <h2 class="pb-3">Desenvolvimento de software</h2>
      <hr class="pb-4">
      <div class="card-group">
        {% assign people = site.data.people | where:"position","dev" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
    <section class="pt-5">
      <h2 class="pb-3">Auxílio organizacional</h2>
      <hr class="pb-4">
      <div class="card-group">
        {% assign people = site.data.people | where:"position","ger-aux" | sort:"name" %}
        {% for person in people %}
          {% include person-grid.html %}
        {% endfor %}
      </div>
    </section>
  </div>
</section>