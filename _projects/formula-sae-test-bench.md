---
layout: page
title: "Senior Capstone Design Project: Formula SAE Test Bench"
description: "Capstone project focused on designing and building a differential test bench to measure torque bias in limited-slip differentials."
img: assets/img/projects/project11.png
importance: 5
category: "Projects"
permalink: /projects/formula-sae-test-bench/
_styles: |
  .project-feature { max-width: 760px; margin: 1.5rem auto; }
  .project-feature img { display: block; width: 100%; height: auto; max-height: 480px; object-fit: contain; }
  .project-gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(min(100%, 220px), 1fr)); gap: 1rem; margin: 1.5rem 0; }
  .project-gallery figure { margin: 0; }
  .project-gallery img { display: block; width: 100%; height: 240px; object-fit: contain; }
---

<div class="project-feature">
  <a href="{{ 'assets/img/projects/project11.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project11.png" alt="Senior Capstone Design Project: Formula SAE Test Bench" class="img-fluid" loading="eager" sizes="(min-width: 800px) 760px, 95vw" %}
  </a>
</div>

This project involved the design, fabrication, and validation of a differential test bench to quantify torque bias in Formula Buckeyes’ limited-slip differential. The system used dual Marathon Electric motors and variable frequency drives (VFDs) to independently drive each half-shaft, with torque measured through RPM and chain-driven loading. Mechanical design, structural analysis, and system integration were completed to ensure accurate and repeatable testing. A data acquisition system was implemented to capture torque response under varying conditions. The final system enabled reliable torque bias measurement, operated below budget constraints, and provided a scalable platform for future drivetrain testing.

## Gallery

Select an image to view it at full size.

<div class="project-gallery">
  <a href="{{ 'assets/img/projects/project11_1.jpg' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project11_1.jpg" alt="Senior Capstone Design Project: Formula SAE Test Bench, additional image 1" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project11_2.jpeg' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project11_2.jpeg" alt="Senior Capstone Design Project: Formula SAE Test Bench, additional image 2" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project11_3.jpeg' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project11_3.jpeg" alt="Senior Capstone Design Project: Formula SAE Test Bench, additional image 3" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project11_4.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project11_4.png" alt="Senior Capstone Design Project: Formula SAE Test Bench, additional image 4" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
</div>

[Back to projects]({{ '/projects/' | relative_url }})
