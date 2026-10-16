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

**ME 395, Industry 4.0 · Northwestern University · 2025**

I built Layerview's core processing pipeline to locate defects in 3D-printed parts by comparing measured geometry with CAD, supporting the team's repair-printing workflow.

**What I built:**

- A MATLAB pipeline for baseline correction, point-cloud filtering, and sampling the reference STL.
- PCA-based initial alignment followed by MATLAB's point-to-plane **iterative closest point (ICP)** registration.
- Geometric error maps and residual analysis to compare the scanned surface with its CAD target.

**Tools:** MATLAB · point-cloud processing · PCA · ICP · STL geometry

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/layerview-icp-alignment.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/layerview-icp-alignment.png" alt="Fringe-projection point cloud and STL reference before and after ICP registration" class="img-fluid" loading="eager" sizes="(min-width: 1000px) 900px, 95vw" %}
  </a>
  <figcaption>Measured geometry and the sampled CAD reference before and after ICP registration. Figure from the team's final presentation.</figcaption>
</figure>

The team's coin-and-letter repair demonstration reduced the reported RMSE from **0.15 mm to 0.10 mm**.

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

- [GitHub repository](https://github.com/ctaylor6/layerview)
- [Final presentation](https://github.com/ctaylor6/layerview/blob/main/docs/layerview-final-presentation.pdf)

**Team:** Natalie Gurganus, Zihan Chen, Lisa Kovacs, Jeremy Lu, and Carter Taylor.

[Back to projects]({{ '/projects/' | relative_url }})
