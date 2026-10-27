---
layout: page
title: "AMPL Triple Machine"
description: "Hybrid forming, CNC milling and laser-wire deposition, with a frame redesigned for APS installation."
img: assets/img/projects/ampl-triple-machine.png
importance: 1
category: "Research"
permalink: /projects/ampl-triple-machine/
role: "Project and capstone team lead"
status: "Under construction"
_styles: |
  .project-feature { max-width: 760px; margin: 1.5rem auto; }
  .project-feature img { display: block; width: 100%; height: auto; max-height: 480px; object-fit: contain; }
  .project-gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(min(100%, 220px), 1fr)); gap: 1rem; margin: 1.5rem 0; }
  .project-gallery figure { margin: 0; }
  .project-gallery img { display: block; width: 100%; height: 240px; object-fit: contain; }
---

I developed the initial concept for AMPL Triple and lead the capstone team building a machine that combines forming, CNC milling and laser-wire deposition. The machine is under construction.

- Led the team in ranking needs and wants, comparing concepts and selecting one machine design.
- Set separate forming and milling stiffness targets for the team's FEA. The design must carry high forming loads while maintaining tool-positioning accuracy for milling and deposition.
- Specified machined mating faces for alignment and bolt preload to carry loads through the joints.
- Led the redesign for Argonne's **Advanced Photon Source (APS)** through layout sketches, design guidance and CAD reviews, addressing the **1.4 m X-ray beam height**, hutch clearance and transport limits.
- The revised design mounts the forming actuator directly into the main beam. Installation is planned around three self-supporting modules.
- Selected a commercial **60 kN Promess actuator** with a **180 mm stroke** and **120 mm/s operating speed**.
- Resized motors on four non-forming axes, reducing quoted cost **by $25k-$30k**.
- Coordinated Aerotech's electrical integration scope and scheduled drawings, fabrication and assembly around supplier lead times.

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/ampl-triple-machine.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/ampl-triple-machine.png" alt="AMPL Triple Machine" class="img-fluid" loading="eager" sizes="(min-width: 800px) 760px, 95vw" %}
  </a>
  <figcaption>Detail CAD: Mohammad Khokha.</figcaption>
</figure>

## Links

- [Full-Size CAD Rendering]({{ 'assets/img/projects/ampl-triple-machine.png' | relative_url }})
- [Capstone Project Overview](https://griffinbraunreiter.com/ampl-triple/)

[Back to projects]({{ '/projects/' | relative_url }})
