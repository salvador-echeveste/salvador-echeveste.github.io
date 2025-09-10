---
layout: about
title: home
permalink: /
subtitle: Machine Learning Research Engineer | PhD in Mechanical Engineering | Bayesian Optimization & Signal Processing Expert

profile:
  align: right
  image: IMG_3235.png
  image_circular: true # crops the image to make it circular
  more_info: >
    <p>Chicago, IL</p>
    <p>sechev6@uic.edu</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page
announcements:
enabled: false # includes a list of news items
scrollable: false # adds a vertical scroll bar if there are more than 3 news items
limit: 0 # leave blank to include all the news in the _news folder
latest_posts:
enabled: false
scrollable: false # adds a vertical scroll bar if there are more than 3 new posts items
limit: 0 # leave blank to include all the blog posts
---

I am a recent PhD graduate from the University of Illinois at Chicago specializing in multi-objective optimization and control systems for wearable robotics. My research bridges machine learning, biomechatronics, and human-computer interaction, with over 5 years developing and deploying real-time optimization algorithms for assistive devices operating in inherently noisy, difficult-to-model environments.
During my doctoral work, I designed and built bilateral hip exoskeletons using quasi-direct drive actuation, developing variable impedance controllers that reduced users' metabolic cost by up to 17.2% and muscle activity (EMG) by 18.2% compared to unassisted movement. My key innovation was implementing a multi-objective Bayesian optimization framework that simultaneously optimized physiological efficiency and user comfort, achieving personalized controller tuning in under 12 minutes—a 10× improvement over traditional methods. This work required tackling the fundamental challenge of input-dependent noise in human physiological responses, where I developed heteroscedastic Gaussian Process models that explicitly captured spatially-varying measurement reliability, improving prediction accuracy by 23-31% over standard approaches.
My expertise centers on extracting meaningful patterns from high-noise, real-time biological signals. I processed 1.77kHz EMG data streams using custom signal processing pipelines that achieved 18.3dB SNR improvement while maintaining sub-10ms latency for control applications. This involved developing Hankel matrix decomposition techniques for artifact removal and Bayesian smoothing methods that balanced noise reduction with physiological signal preservation. The real-time constraints of human-in-the-loop control, combined with the inherent variability of biological systems, required innovative approaches to uncertainty quantification and adaptive sampling strategies that focused computational resources on regions with reliable human responses.
Through 11-subject clinical studies, I discovered fundamental trade-offs between EMG minimization and user preference using Pareto front analysis, demonstrating that these objectives often conflict in human-centered design. My use of Expected Hypervolume Improvement enabled efficient exploration of this multi-objective space without requiring a priori weight specification, revealing task-specific control strategies that emerged consistently across subjects despite high inter-subject variability exceeding 100% for certain parameters.
I am seeking challenging opportunities in machine learning where I can apply my expertise in probabilistic modeling, signal processing, and optimization to complex, noisy real-time systems. My experience with heteroscedastic modeling, uncertainty quantification, and human-in-the-loop optimization positions me well for tackling difficult problems in robotics, biomedical systems, financial modeling, or any domain where traditional assumptions of constant noise and static environments break down. I thrive on developing algorithms that bridge the gap between theoretical elegance and the messy reality of deployed systems operating under real-world constraints.
