---
layout: page
title: "Deterministic Keyhole-Collapse Detection"
description: "I built deterministic keyhole-collapse detection from thermal-emission signals, with no training dataset or pretrained ML model."
img: assets/img/projects/lpbf-detector-comparison.png
importance: 0
category: "Projects"
permalink: /projects/lpbf-collapse-detection/
_styles: |
  .project-feature { max-width: 900px; margin: 1.5rem auto; }
  .project-feature img { display: block; width: 100%; height: auto; object-fit: contain; }
  .project-feature figcaption { font-size: 0.875rem; margin-top: 0.5rem; }
  .project-feature.embedding { max-width: 480px; }
---

**AI for Manufacturing · Course project**

I developed a **deterministic method for keyhole-collapse detection** in laser powder bed fusion to remove the need for labeled training data and a trained machine-learning model.

**What I built:**

- Signal filtering and sliding-window extraction of physical features from thermal-emission measurements.
- PCA and Mahalanobis-distance scoring calculated directly from the input signal: **no separate training dataset or pretrained ML model**.
- Time-aligned scores and candidate-event visualizations, compared with my PI-TSAD method as a reference.

**Tools:** Python · NumPy · SciPy · statistical signal processing · PCA · Matplotlib

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/lpbf-detector-comparison.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/lpbf-detector-comparison.png" alt="Thermal-emission signal with PCA and random-forest event predictions and their corresponding scores" class="img-fluid" loading="eager" sizes="(min-width: 1000px) 900px, 95vw" %}
  </a>
  <figcaption>Deterministic statistical scoring compared with my PI-TSAD baseline. The random forest is shown only for comparison; it is not used by this detector.</figcaption>
</figure>

<figure class="project-feature embedding">
  <a href="{{ 'assets/img/projects/lpbf-feature-embedding.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/lpbf-feature-embedding.png" alt="UMAP embedding of window features with supplied collapse labels shown in red" class="img-fluid" loading="lazy" sizes="480px" %}
  </a>
  <figcaption>Exploratory feature visualization from the study. This embedding is not part of the deterministic detector.</figcaption>
</figure>

The code calculates PCA statistics from the signal being analyzed. The offline demo uses synthetic input; experimental datasets and trained models are not distributed.

[GitHub repository](https://github.com/ctaylor6/deterministic-keyhole-collapse-detection) · [Back to projects]({{ '/projects/' | relative_url }})
