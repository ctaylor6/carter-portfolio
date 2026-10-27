---
layout: page
title: "APS Beamline: Collecting Ground Truth"
description: "X-ray and photodiode experiments connecting optical signals with melt-pool and pore behavior."
img: assets/img/projects/aps-experimental-setup.jpg
importance: 3
category: "Research"
permalink: /projects/aps-ground-truth/
_styles: |
  .project-gallery { display: grid; grid-template-columns: repeat(auto-fit, minmax(min(100%, 280px), 1fr)); gap: 1.5rem; margin: 1.5rem 0; }
  .project-gallery figure { margin: 0; }
  .project-gallery img { display: block; width: 100%; height: 440px; object-fit: contain; }
  .project-gallery figcaption { font-size: 0.875rem; margin-top: 0.5rem; }
---

At Argonne's Advanced Photon Source (APS), X-ray imaging reveals melt-pool motion and pore formation that an optical sensor cannot see directly. I helped collect X-ray and photodiode data at **APS 32-ID in October 2026** to connect the optical signals with that ground truth.

- Set photodiode sampling requirements relative to the X-ray camera with the optics and acquisition team.
- Specified a **15 ms capture window** using track length, scan speed and prior experimental records.
- Collected data with the team under fixed conditions and **step, impulse and ramp changes in laser power**.
- Tested **wrought and as-built substrates** across beam modes and scan speeds, with run records linking conditions and sample IDs to repeats and observations.

These experiments provide paired measurements for studying how optical signals relate to melt-pool behavior and pore interactions. The October campaign is separate from the earlier dataset used to validate [PI-TSAD]({{ '/projects/pi-tsad/' | relative_url }}).

<div class="project-gallery">
  <figure>
    <a href="{{ 'assets/img/projects/aps-experimental-setup.jpg' | relative_url }}">
      {% include figure.liquid path="assets/img/projects/aps-experimental-setup.jpg" alt="APS 32-ID setup with a stainless process replicator at center-left and a white infrared camera to its right" class="img-fluid" loading="eager" sizes="(min-width: 800px) 420px, 95vw" %}
    </a>
    <figcaption>APS 32-ID setup. The process replicator is at center-left, with the IR camera aimed toward its chamber from the right.</figcaption>
  </figure>
  <figure>
    <a href="{{ 'assets/img/projects/aps-experiment-team.png' | relative_url }}">
      {% include figure.liquid path="assets/img/projects/aps-experiment-team.png" alt="Four members of the APS experiment team in the control room, with Carter Taylor at the far right in a gray fleece" class="img-fluid" loading="lazy" sizes="(min-width: 800px) 420px, 95vw" %}
    </a>
    <figcaption>Our experiment team in the control room. I am at the far right.</figcaption>
  </figure>
</div>

[Experiment record](https://doi.org/10.46936/APS-196273/60018545) · [Back to projects]({{ '/projects/' | relative_url }})
