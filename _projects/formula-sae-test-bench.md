---
layout: page
title: "Senior Capstone Design Project: Formula SAE Test Bench"
description: "A motor-driven bench for measuring torque bias in the Formula Buckeyes limited-slip differential."
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

I helped design, fabricate and validate a torque-bias-ratio test bench for Formula Buckeyes as part of a three-person capstone team.

- Compared in-car, static and motor-driven tests before selecting a motor-driven bench.
- Used **two 3 hp, three-phase motors**, variable frequency drives and chain drives to load the differential.
- Checked the mounting platform for yielding with **finite-element analysis** and added an emergency stop.
- Implemented **LabVIEW data acquisition** to record differential torque.
- Completed the bench for **less than $2,000** and collected torque data to evaluate torque bias ratio and support future drivetrain testing.

Capstone team: Carter Taylor, Joe Onderko and Cooper Sautter. Advisor: Shawn Midlam-Mohler.

<div class="project-feature">
  <a href="{{ 'assets/img/projects/project11.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project11.png" alt="Senior Capstone Design Project: Formula SAE Test Bench" class="img-fluid" loading="eager" sizes="(min-width: 800px) 760px, 95vw" %}
  </a>
</div>

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
