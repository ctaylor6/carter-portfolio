---
layout: page
title: "Layerview: 3D Print Inspection and Repair"
description: "Built the core MATLAB processing and ICP registration pipeline for fringe-projection inspection and repair of 3D-printed parts."
img: assets/img/projects/layerview-icp-alignment.png
importance: 1
category: "Projects"
permalink: /projects/layerview/
role: "Core processing pipeline and ICP registration"
_styles: |
  .project-feature { max-width: 900px; margin: 1.5rem auto; }
  .project-feature img { display: block; width: 100%; height: auto; object-fit: contain; }
  .project-feature figcaption, .project-gallery figcaption { font-size: 0.875rem; margin-top: 0.5rem; }
  .project-gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(min(100%, 300px), 1fr)); gap: 1rem; margin: 1.5rem 0; }
  .project-gallery figure { margin: 0; }
  .project-gallery img { display: block; width: 100%; height: auto; object-fit: contain; }
---

**Role:** Core processing pipeline and ICP registration<br>
**Context:** ME 395, Industry 4.0 · Northwestern University · 2025

I built the core MATLAB processing pipeline for Layerview, a team project connecting fringe-projection scans to geometric inspection and repair of 3D-printed parts. My work covered point-cloud filtering, CAD reference sampling, initial alignment, integration of iterative closest point (ICP) registration, and geometric error analysis.

The team used a camera and projector to measure parts on an Ender 3 Pro. The workflow compared the measured surface with its intended geometry, identified missing material, and generated an STL patch for repair printing.

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/layerview-icp-alignment.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/layerview-icp-alignment.png" alt="Fringe-projection point cloud and STL reference before and after ICP registration" class="img-fluid" loading="eager" sizes="(min-width: 1000px) 900px, 95vw" %}
  </a>
  <figcaption>Measured geometry and the sampled CAD reference before and after ICP registration. Figure from the team's final presentation.</figcaption>
</figure>

## My contribution

I developed the processing stages that turn noisy scan data into an aligned geometric comparison. The pipeline uses a baseline scan to remove the height offset, filters outliers and separates the printed feature from its base, and samples the reference STL into a point cloud. PCA provides the initial orientation before MATLAB's point-to-plane ICP refines the registration. Nearest-neighbor residuals then produce error maps and distributions for evaluating the part.

The repair workflow builds on that comparison: points representing missing geometry define a boundary that is extruded and triangulated into a repair STL. The demonstration focused on simple coin-and-letter geometries.

## Demonstration

The final presentation reports control-case registration RMSE values of **0.082–0.085 mm**. In the illustrated repair comparison, the reported RMSE decreased from **0.15 mm to 0.10 mm**. These results are specific to the course-project demonstration.

<div class="project-gallery">
  <figure>
    <a href="{{ 'assets/img/projects/layerview-defect-residuals.jpg' | relative_url }}">
      {% include figure.liquid path="assets/img/projects/layerview-defect-residuals.jpg" alt="Geometric residual map of the defective printed part" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 440px, 95vw" %}
    </a>
    <figcaption>Before repair: reported RMSE of 0.15 mm.</figcaption>
  </figure>
  <figure>
    <a href="{{ 'assets/img/projects/layerview-repair-residuals.jpg' | relative_url }}">
      {% include figure.liquid path="assets/img/projects/layerview-repair-residuals.jpg" alt="Geometric residual map after the repair demonstration" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 440px, 95vw" %}
    </a>
    <figcaption>After repair: reported RMSE of 0.10 mm. The two plots use different color scales.</figcaption>
  </figure>
</div>

## Code and presentation

- [GitHub repository](https://github.com/ctaylor6/layerview)
- [Final presentation](https://github.com/ctaylor6/layerview/blob/main/docs/layerview-final-presentation.pdf)

**Team:** Natalie Gurganus, Zihan Chen, Lisa Kovacs, Jeremy Lu, and Carter Taylor.

[Back to projects]({{ '/projects/' | relative_url }})
