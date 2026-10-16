---
layout: page
title: "CFD of Polymer Flow and Melting in a 3D-Printer Nozzle"
description: "I built the ANSYS Fluent pipeline and melting/solidification model to study PLA flow, heating, and nozzle design."
img: assets/img/projects/cfd-pla-viscosity.png
importance: 2
category: "Projects"
permalink: /projects/fdm-nozzle-cfd/
_styles: |
  .project-feature { max-width: 900px; margin: 1.5rem auto; }
  .project-feature.constitutive { max-width: 560px; }
  .project-feature img { display: block; width: 100%; height: auto; object-fit: contain; background: #fff; }
  .project-feature figcaption { font-size: 0.875rem; margin-top: 0.5rem; }
---

**ME 378 · Northwestern University · March 2025**

I built the **core CFD pipeline and melting/solidification model** to study how nozzle geometry and heating affect PLA extrusion, with the goal of reducing extrusion pressure while maintaining suitable flow conditions for printing.

**What I built:**

- A 2D axisymmetric ANSYS Fluent workflow coupling non-Newtonian flow and heat transfer.
- Viscosity user-defined functions to capture PLA's temperature and shear-rate dependence.
- A melting/solidification model using enthalpy-porosity and temperature-dependent heat capacity to resolve the transition from solid filament to flowing polymer.

**Tools:** ANSYS Fluent · CFD · viscosity UDFs · enthalpy-porosity modeling

My teammates carried out validation comparisons against published simulations and grid-convergence analysis. My contribution was developing the simulation pipeline and material models used in that work.

<figure class="project-feature constitutive">
  <a href="{{ 'assets/img/projects/cfd-pla-viscosity.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/cfd-pla-viscosity.png" alt="Carreau-Yasuda PLA viscosity surface showing dependence on temperature and shear rate" class="img-fluid" loading="eager" sizes="560px" %}
  </a>
  <figcaption>Temperature- and shear-dependent PLA viscosity used in the melting/solidification extension.</figcaption>
</figure>

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/cfd-liquid-fraction.jpg' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/cfd-liquid-fraction.jpg" alt="Liquid-fraction field showing solid PLA melting as it moves through the heated domain" class="img-fluid" loading="lazy" sizes="(min-width: 1000px) 900px, 95vw" %}
  </a>
  <figcaption>The liquid-fraction field resolves the solid-to-liquid transition upstream of the nozzle. Figures from the team's final presentation.</figcaption>
</figure>

**Team:** Jack Nulisch, Carter Taylor, Garrett Mathesen, and Natasha Van Dam.

[Back to projects]({{ '/projects/' | relative_url }})
