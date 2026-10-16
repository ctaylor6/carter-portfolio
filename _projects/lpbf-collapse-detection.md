---
layout: page
title: "PCA-Based Melt-Pool Collapse Detection"
description: "I built a Python workflow that turns thermal-emission signals into physics-based features and anomaly scores for laser powder bed fusion."
img: assets/img/projects/lpbf-detector-comparison.png
importance: 2
category: "Projects"
permalink: /projects/lpbf-collapse-detection/
_styles: |
  .project-feature { max-width: 900px; margin: 1.5rem auto; }
  .project-feature img { display: block; width: 100%; height: auto; object-fit: contain; }
  .project-feature figcaption { font-size: 0.875rem; margin-top: 0.5rem; }
  .project-feature.embedding { max-width: 480px; }
---

**AI for Manufacturing · Course project**

Building on my [PI-TSAD work](https://github.com/ctaylor6/PI-TSAD), I explored whether PCA-based analysis could identify melt-pool collapse from thermal-emission signals using a small set of interpretable features.

**What I built:**

- Signal filtering and sliding-window extraction of amplitude, variability, and frequency-band features from 200 kHz measurements.
- PCA and Mahalanobis-distance scoring to identify unusual windows and compare them with supplied collapse labels.
- Comparisons with my PI-TSAD random-forest model, plus UMAP visualizations of the feature space.

**Tools:** Python · NumPy · SciPy · pandas · scikit-learn · UMAP · Matplotlib

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/lpbf-detector-comparison.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/lpbf-detector-comparison.png" alt="Thermal-emission signal with PCA and random-forest event predictions and their corresponding scores" class="img-fluid" loading="eager" sizes="(min-width: 1000px) 900px, 95vw" %}
  </a>
  <figcaption>PCA-based scores compared with my PI-TSAD random-forest baseline. Markers show each method's predictions, not independently confirmed defects.</figcaption>
</figure>

<figure class="project-feature embedding">
  <a href="{{ 'assets/img/projects/lpbf-feature-embedding.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/lpbf-feature-embedding.png" alt="UMAP embedding of window features with supplied collapse labels shown in red" class="img-fluid" loading="lazy" sizes="480px" %}
  </a>
  <figcaption>UMAP feature-space visualization, with supplied collapse-window labels in red.</figcaption>
</figure>

This was an offline exploratory study. The repository includes the original notebook sources and a cleaned, tested PCA demo.

[GitHub repository](https://github.com/ctaylor6/lpbf-collapse-detection) · [Back to projects]({{ '/projects/' | relative_url }})
