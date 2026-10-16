---
layout: page
title: "Pore Closure in Additively Manufactured Titanium"
description: "I independently built an Abaqus model to study how forming closes pores in printed Ti-6Al-4V and how much deformation remains after unloading."
img: assets/img/projects/titanium-pore-rve.png
importance: 3
category: "Projects"
permalink: /projects/titanium-pore-closure/
_styles: |
  .project-feature { max-width: 900px; margin: 1.5rem auto; }
  .project-feature.geometry { max-width: 320px; }
  .project-feature img { display: block; width: 100%; height: auto; object-fit: contain; background: #fff; }
  .project-feature figcaption { font-size: 0.875rem; margin-top: 0.5rem; }
---

**ME/CEE 426, Advanced Finite Elements · Northwestern University · March 2025**

**Individual project — all modeling, verification, analysis, and reporting by Carter Taylor.**

I built a finite element model to investigate whether mechanical forming could close gas pores in directed-energy-deposited Ti-6Al-4V, supporting the development of hybrid additive and forming processes.

**What I built:**

- A quarter-symmetry representative volume element in Abaqus/Explicit, with a spherical pore and Johnson–Cook plasticity.
- Mesh-convergence and energy checks, followed by loading/unloading simulations to measure pore closure and springback.
- Studies of forming depth, temperature, boundary conditions, and ductile damage to assess closure, forming force, and residual stress.

**Tools:** Abaqus/Explicit · finite element analysis · Johnson–Cook plasticity and damage

<figure class="project-feature geometry">
  <a href="{{ 'assets/img/projects/titanium-pore-rve.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/titanium-pore-rve.png" alt="Quarter-symmetry Abaqus model of a titanium representative volume element containing a spherical pore" class="img-fluid" loading="eager" sizes="320px" %}
  </a>
  <figcaption>The representative volume element and symmetry model used in the study.</figcaption>
</figure>

In the room-temperature model, increasing displacement from **0.375 to 0.5 mm** required about **18% more force** with little additional benefit to pore closure after unloading. These are numerical feasibility results for the modeled geometry and boundary conditions.

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/titanium-pore-recovery.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/titanium-pore-recovery.png" alt="Undeformed, loaded, and unloaded pore profiles for forming displacements of 0.25, 0.375, and 0.5 millimeters" class="img-fluid" loading="lazy" sizes="(min-width: 1000px) 900px, 95vw" %}
  </a>
  <figcaption>Pore profiles before loading, under load, and after unloading at 0.25, 0.375, and 0.5 mm displacement, from left to right.</figcaption>
</figure>

[Back to projects]({{ '/projects/' | relative_url }})
