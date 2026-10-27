---
layout: page
title: "PI-TSAD: Detecting Keyhole Collapse"
description: "Photodiode-based detection validated against synchrotron X-ray labels and transferred to eight commercial builds without retraining."
img: assets/img/projects/pi-tsad-aps-validation.png
importance: 0
category: "Research"
permalink: /projects/pi-tsad/
_styles: |
  .project-feature { max-width: 900px; margin: 1.5rem auto; }
  .project-feature img { display: block; width: 100%; height: auto; object-fit: contain; }
  .project-feature figcaption { font-size: 0.875rem; margin-top: 0.5rem; }
---

I developed PI-TSAD, a physically informed time-series anomaly detector, to identify keyhole collapse from photodiode signals during laser powder bed fusion.

- Analyzed **200 kHz photodiode data** and selected a **0.25-30 kHz filter** to isolate melt-pool dynamics.
- Extracted statistical and frequency-domain features and trained a **Random Forest classifier** to identify collapse events.
- Validated event timing on **four held-out melt tracks** against synchrotron X-ray labels from the Advanced Photon Source (APS).
- Transferred the detector to **eight AlSi10Mg builds on a commercial DMG MORI LASERTEC 12 SLM without retraining**.

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/pi-tsad-aps-validation.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/pi-tsad-aps-validation.png" alt="PI-TSAD collapse-event predictions compared with X-ray ground-truth labels for four held-out melt tracks" class="img-fluid" loading="eager" sizes="(min-width: 1000px) 900px, 95vw" %}
  </a>
  <figcaption>Collapse predictions for four held-out tracks, compared with synchrotron X-ray labels. Figure from the PI-TSAD paper.</figcaption>
</figure>

Across the commercial builds, anomaly counts followed the CT pore-count trend. The lack-of-fusion sample exposed a limitation: a detector trained on keyhole collapse does not capture every mechanism that produces porosity.

<figure class="project-feature">
  <a href="{{ 'assets/img/projects/pi-tsad-commercial-builds.png' | relative_url }}">
    {% include figure.liquid path="assets/img/projects/pi-tsad-commercial-builds.png" alt="PI-TSAD anomaly counts and baseline peak counts compared with CT pore counts for eight AlSi10Mg builds" class="img-fluid" loading="lazy" sizes="(min-width: 1000px) 900px, 95vw" %}
  </a>
  <figcaption>Comparison with CT measurements across eight builds. Figure from the PI-TSAD paper.</figcaption>
</figure>

This first-author work was published in the [Journal of Manufacturing Processes (2026)](https://doi.org/10.1016/j.jmapro.2026.04.026) and received the NAMRC Outstanding Paper Award in Manufacturing Processes and Student Research Presentation Award.

[Read the paper](https://doi.org/10.1016/j.jmapro.2026.04.026) · [Code](https://github.com/ctaylor6/PI-TSAD)

[Back to projects]({{ '/projects/' | relative_url }})
