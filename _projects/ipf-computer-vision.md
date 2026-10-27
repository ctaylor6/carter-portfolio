---
layout: page
title: "Incremental Profile Forming: Computer Vision System"
description: "Three laser line sensors measure tube geometry during incremental profile forming."
img: assets/img/projects/project10_1.png
importance: 3
category: "Research"
permalink: /projects/ipf-computer-vision/
_styles: |
  .project-feature { max-width: 760px; margin: 1.5rem auto; }
  .project-feature img { display: block; width: 100%; height: auto; max-height: 480px; object-fit: contain; }
  .project-gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(min(100%, 220px), 1fr)); gap: 1rem; margin: 1.5rem 0; }
  .project-gallery figure { margin: 0; }
  .project-gallery img { display: block; width: 100%; height: 240px; object-fit: contain; }
---

I developed an alignment fixture and MATLAB calibration code for three laser line sensors to measure tube geometry during incremental profile forming (IPF).

- Designed the fixture to establish the sensor planes and a common global origin.
- Replaced small alignment holes with raised scan features that could be machined in-house.
- Developed coordinate transformations using **Taubin circle fitting**, rotation and translation. Alignment and transformation error was **below 0.20 mm**.
- Compared **three indented specimens** against Keyence reference scans using **point-to-plane iterative closest point (ICP)** alignment.
- Measured **3D root-mean-square error (RMSE) of 0.0356-0.0511 mm** and **profile RMSE of 0.0150-0.0160 mm** across the three specimens.

<div class="project-feature">
  <a href="{{ 'assets/img/projects/project10_1.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project10_1.png" alt="Incremental Profile Forming: Computer Vision System" class="img-fluid" loading="eager" sizes="(min-width: 800px) 760px, 95vw" %}
  </a>
</div>

## Links

- [Video of the Process](https://youtu.be/ODje2JpOuVM)
- [Undergraduate Honors Thesis](https://kb.osu.edu/server/api/core/bitstreams/e8608f61-c2b8-42cd-9044-86337d9b4eda/content)

## Gallery

Select an image to view it at full size.

<div class="project-gallery">
  <a href="{{ 'assets/img/projects/project10.jpg' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project10.jpg" alt="Incremental Profile Forming: Computer Vision System, additional image 1" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project10_2.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project10_2.png" alt="Incremental Profile Forming: Computer Vision System, additional image 2" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project10_3.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project10_3.png" alt="Incremental Profile Forming: Computer Vision System, additional image 3" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project10_4.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project10_4.png" alt="Incremental Profile Forming: Computer Vision System, additional image 4" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project10_5.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project10_5.png" alt="Incremental Profile Forming: Computer Vision System, additional image 5" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project10_6.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project10_6.png" alt="Incremental Profile Forming: Computer Vision System, additional image 6" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
  <a href="{{ 'assets/img/projects/project10_7.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/project10_7.png" alt="Incremental Profile Forming: Computer Vision System, additional image 7" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 380px, 95vw" %}
  </a>
</div>

[Back to projects]({{ '/projects/' | relative_url }})
