---
layout: page
permalink: /publications/
title: publications
description: Papers, preprints, and earlier work.
nav: true
nav_order: 2
---

<link rel="stylesheet" href="{{ '/assets/css/publication-previews.css' | relative_url | bust_file_cache }}">

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
