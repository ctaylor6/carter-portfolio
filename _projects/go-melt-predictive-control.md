---
layout: page
title: "GO-MELT: Thermal Modeling and Predictive Control"
description: "Thermal FEA, recurrent process models, and predictive control of laser power and beam mode in simulation."
img: assets/img/projects/go-melt-trained-controller-comparison.png
importance: 2
category: "Research"
permalink: /projects/go-melt-predictive-control/
_styles: |
  .project-feature { max-width: 580px; margin: 1.5rem auto; }
  .project-feature img { display: block; width: 100%; height: auto; object-fit: contain; }
  .project-feature figcaption { font-size: 0.875rem; margin-top: 0.5rem; }
---

I use GO-MELT thermal simulations to develop predictive controllers that adjust laser power and beam mode to regulate melt-pool geometry and photodiode temperature.

- Configured locally refined meshes, laser heat sources, and thermal boundary conditions in the existing GO-MELT finite-element solver.
- Developed a scheme to filter experimental data for the team's simulation calibration and assessed mesh sensitivity.
- Generated temperature and melt-pool histories to train recurrent prediction models using long short-term memory (LSTM) networks.
- Developed model predictive control (MPC) and trained differentiable predictive control (DPC) for coordinated power and beam-mode commands.

In the simulation below, joint MPC and trained DPC followed the large width changes that the power-only controllers missed, while also regulating depth and temperature.

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/go-melt-trained-controller-comparison.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/go-melt-trained-controller-comparison.png" alt="Trained controller comparison showing melt-pool depth, width, photodiode temperature, laser power, and beam mode over time" class="img-fluid" loading="eager" sizes="(min-width: 640px) 580px, 95vw" %}
  </a>
  <figcaption>Simulation comparison of joint MPC, trained DPC, power-only MPC, and PID. The lower panels show the commanded laser power and beam mode.</figcaption>
</figure>

[View the full-size figure]({{ 'assets/img/projects/go-melt-trained-controller-comparison.png' | relative_url }})

[Back to projects]({{ '/projects/' | relative_url }})
