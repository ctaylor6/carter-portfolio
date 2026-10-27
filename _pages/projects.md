---
layout: page
title: projects
permalink: /projects/
description: Research, engineering projects, and things I have built and restored.
nav: true
nav_order: 3
display_categories: [Research, Projects, Entrepreneurship]
horizontal: false
_styles: |
  .projects h2.category { color: var(--global-text-color); text-align: left; }
  .projects .card-title { font-size: 1.125rem; line-height: 1.4; }
  .projects .card-text { font-size: 0.875rem; line-height: 1.6; }
  .projects .card-img-top { width: 100%; height: 190px; object-fit: cover; }
  .projects a[href$="/ampl-triple-machine/"] .card-img-top { object-position: center; object-fit: contain; }
  .projects a[href$="/layerview/"] .card-img-top { object-fit: contain; background: #000; }
  .projects a[href$="/lpbf-collapse-detection/"] .card-img-top { object-fit: contain; background: #fff; }
  .projects a[href$="/go-melt-predictive-control/"] .card-img-top { object-fit: contain; background: #fff; }
  .projects a[href$="/pi-tsad/"] .card-img-top { object-fit: contain; background: #fff; }
  .projects a[href$="/fdm-nozzle-cfd/"] .card-img-top { object-fit: contain; background: #fff; }
  .projects a[href$="/titanium-pore-closure/"] .card-img-top { object-fit: contain; background: #fff; }
  .projects a[href$="/owens-corning-research/"] .card-img-top { object-position: center center; }
  .projects a[href$="/ipf-computer-vision/"] .card-img-top { object-position: center center; }
  .projects a[href$="/ipf-physics-modeling/"] .card-img-top { object-position: center center; }
  .projects a[href$="/formula-sae-test-bench/"] .card-img-top { object-position: center center; }
  .projects a[href$="/makeathon-solar-panel/"] .card-img-top { object-position: center center; }
  .projects a[href$="/industrial-water-supply/"] .card-img-top { object-position: center center; }
  .projects a[href$="/animatronic-restoration/"] .card-img-top { object-position: center 12%; }
  .projects a[href$="/cushman-scooter-restoration/"] .card-img-top { object-position: center 62%; }
  .projects a[href$="/original-coffee-pellet/"] .card-img-top { object-position: center 72%; }
---

<div class="projects">
  {% if site.enable_project_categories and page.display_categories %}
    {% for category in page.display_categories %}
      <h2 id="{{ category | slugify }}" class="category">{{ category }}</h2>
      {% assign categorized_projects = site.projects | where: "category", category %}
      {% assign sorted_projects = categorized_projects | sort: "importance" %}
      <div class="row row-cols-1 row-cols-md-3">
        {% for project in sorted_projects %}
          {% include projects.liquid %}
        {% endfor %}
      </div>
    {% endfor %}
  {% else %}
    {% assign sorted_projects = site.projects | sort: "importance" %}
    <div class="row row-cols-1 row-cols-md-3">
      {% for project in sorted_projects %}
        {% include projects.liquid %}
      {% endfor %}
    </div>
  {% endif %}
</div>
