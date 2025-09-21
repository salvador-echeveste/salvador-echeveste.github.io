---
layout: page
title: EMG Signal Enhancement
description: Hankel-based Bayesian learning with multi-objective optimization for EMG denoising
img: /assets/img/EMG_enhancement_icon.png
importance: 1
category: work
related_publications: true
paper: /assets/pdf/Echeveste(2025)EMG_Signal_enhancement_via_Hankelbased_bayesian_learning.pdf
github: https://github.com/salvador-echeveste/signal_enhancement
---

## Project Overview

Electromyography (EMG) signals are crucial for diagnosing neuromuscular conditions and controlling assistive devices, but they're plagued by noise that obscures clinically important features. We developed an automated framework that enhances EMG quality while preserving the subtle transient features that doctors and devices need to see.

### Key Innovation
Unlike traditional filters that force a trade-off between removing noise and keeping real signal content, our method **decouples these objectives** using multi-objective Bayesian optimization. The result: **108.7% improvement** in signal quality metrics while maintaining signal fidelity.

<p>
  <a href="{{ page.github }}" target="_blank" rel="noopener" style="text-decoration:none;">
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

## Technical Approach

### The Pipeline
<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/overview_hankel.png" title="EMG enhancement & MOBO workflow" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Complete signal enhancement pipeline with multi-objective optimization</div>
  </div>
</div>

Our framework combines four key components:
1. **Hankel Matrix Decomposition** - Embeds time-series data to separate signal from noise
2. **Bayesian Koopman Regression** - Learns underlying dynamics with uncertainty quantification
3. **Weighted Signal Fusion** - Optimally combines reconstructed and predicted signals
4. **Makima Median Smoothing** - Final refinement preserving transient features

### Signal Processing Stages
<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/signal_hankel.png" title="Processing stages for one EMG channel" class="img-fluid rounded z-depth-1" %}
    <div class="caption">Signal transformation through each processing stage</div>
  </div>
</div>

## Key Results

### Breaking the Trade-off
Traditional EMG processing forces you to choose: remove noise OR preserve signal features. Our method achieves both:

<div class="row">
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/correlation_hankel.png" title="Correlation SNR vs SSIM" class="img-fluid rounded z-depth-1" %}
    <div class="caption"><b>Decoupled objectives:</b> Traditional methods (gray) show strong negative correlation (r=-0.64) between noise reduction and signal fidelity. Our method (blue) breaks this trade-off (r≈0).</div>
  </div>
  <div class="col-sm-6 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/results_all_hankel.png" title="Overall performance comparison" class="img-fluid rounded z-depth-1" %}
    <div class="caption"><b>Superior performance:</b> 108.7% improvement in combined metrics (p=0.028) and 11.4% gain in normalized joint fidelity (p=0.001)</div>
  </div>
</div>


## Why This Matters

### Clinical Impact
- **Better Diagnosis:** Cleaner signals help doctors identify neuromuscular conditions more accurately
- **Improved Prosthetics:** Enhanced EMG enables more precise control of assistive devices
- **Real-time Processing:** Automated parameter tuning eliminates manual trial-and-error

### Technical Innovation
- **Multi-objective Optimization:** First application of MOBO to EMG enhancement
- **Interpretable Framework:** Unlike black-box deep learning, our method is fully explainable
- **Automated Tuning:** No manual parameter selection needed

## Implementation Details

### Parameter Space
The framework optimizes 5 key parameters automatically:
- Embedding dimension (d): 50-150
- SVD rank (r): 3-10  
- Regularization variances (σ², τ²)
- Fusion weight (w): 0-1

### Optimization Strategy
- **Gaussian Process Surrogates** model objective functions
- **Expected Hypervolume Improvement** guides exploration
- **Pareto Front** extraction preserves all optimal trade-offs

## Dataset & Validation

Tested on 10 healthy adults performing:
- Level-ground walking
- Bodyweight squatting
- 4 muscle groups: Rectus Femoris, Biceps Femoris, Gastrocnemius, Gluteus Maximus
- 2 kHz sampling rate with SENIAM electrode placement

## Publications & Resources

📄 [Full Paper (PDF)]({{ page.paper }})

📊 [Code & Implementation]({{ page.github }})

📐 [Mathematical Details](#technical-approach)

## Team

**Lead Researcher:** Salvador Echeveste  
**Co-authors:** Chunming Yang, Pranav A. Bhounsule  
**Institution:** University of Illinois at Chicago  
**Department:** Mechanical and Industrial Engineering  
**Contact:** sechev6@uic.edu

---

*This work advances the state-of-the-art in biomedical signal processing, with applications in rehabilitation engineering, clinical diagnostics, and human-machine interfaces.*
