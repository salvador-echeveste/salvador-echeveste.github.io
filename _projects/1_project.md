---
layout: page
title: EMG signal enhancement
description: Hankel-based Bayesian learning with multi-objective optimization for EMG denoising
img: /assets/EMG_enhancement_icon.png
importance: 1
category: work
related_publications: true
paper: /assets/img/EMG_Signal_Enhancement_via_Multi_Objective_Optimization_of_Hankel_Based_Bayesian_Learning.pdf
overview: /assets/img/OVERVIEW3.pdf
github: https://github.com/salvador-echeveste/signal_enhancement
---
<p>
  <a href="{{ page.github }}" target="_blank" rel="noopener" style="text-decoration:none;">
    <!-- GitHub SVG icon -->
    <svg height="16" width="16" viewBox="0 0 16 16" aria-hidden="true" style="vertical-align: text-bottom; margin-right:6px;">
      <path fill="currentColor" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38
      0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52
      -.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89
      -3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.01.08-2.11 0 0 .67-.21 2.2.82.64-.18 1.32-.27
      2-.27s1.36.09 2 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.91.08 2.11.51.56.82 1.27.82 2.15
      0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013
      8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z" />
    </svg>
    View code on GitHub
  </a>
</p>
## Figures & downloads

Below are the figures used in the manuscript. Click the captions to open the original PDF figure (all files assumed to live in `assets/img/`).

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/OVERVIEW3.jpg" title="Overview: EMG enhancement & MOBO workflow (click caption to open PDF)" class="img-fluid rounded z-depth-1" %}
    <div class="caption"><a href="/assets/img/OVERVIEW3.pdf" target="_blank">Figure: Overview — pipeline & optimization (OVERVIEW3.pdf)</a></div>
  </div>
</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/SIGNAL2.jpg" title="Processing stages for one EMG channel (click caption to open PDF)" class="img-fluid rounded z-depth-1" %}
    <div class="caption"><a href="/assets/img/SIGNAL2.pdf" target="_blank">Figure: Processing stages / smoother (SIGNAL2.pdf)</a></div>
  </div>
</div>

<div class="row">
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/CORR.jpg" title="Correlation SNR vs SSIM (click caption to open PDF)" class="img-fluid rounded z-depth-1" %}
    <div class="caption"><a href="/assets/img/CORR.pdf" target="_blank">Figure: Correlation scatter (CORR.pdf)</a></div>
  </div>
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/RES_ALL.jpg" title="Overall SGM & joint metric comparison (click caption to open PDF)" class="img-fluid rounded z-depth-1" %}
    <div class="caption"><a href="/assets/img/RES_ALL.pdf" target="_blank">Figure: All-subject comparison (RES_ALL.pdf)</a></div>
  </div>
</div>

<div class="row">
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/RES_MUS.jpg" title="Muscle-specific results (click caption to open PDF)" class="img-fluid rounded z-depth-1" %}
    <div class="caption"><a href="/assets/img/RES_MUS.pdf" target="_blank">Figure: Muscle-specific results (RES_MUS.pdf)</a></div>
  </div>
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/RES_ACT.jpg" title="Activity-specific results (click caption to open PDF)" class="img-fluid rounded z-depth-1" %}
    <div class="caption"><a href="/assets/img/RES_ACT.pdf" target="_blank">Figure: Activity-specific results (RES_ACT.pdf)</a></div>
  </div>
</div>

---
