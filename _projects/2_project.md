---
layout: page
title: What Makes Amherst Look Like Amherst?
description: 60K-frame geospatial vision study on the signals that distinguish Amherst, MA from other college towns.
img: assets/img/3.jpg
importance: 2
category: work
github: https://github.com/aeyanashraf/What-makes-Amherst-look-like-Amherst
---

This project explores whether we can teach a model to understand the “feel” of Amherst, MA by learning from its built environment. The pipeline covers dataset curation, geospatial augmentation, interpretable CNN training, and qualitative analyses that surface what the models actually latch onto.

### Dataset + labeling
- Pulled >60K street-level frames across seasons, stratified to balance residential, downtown, and campus viewpoints.
- Normalized lighting/seasonality via augmentation and created “contrast sets” pairing Amherst with peer college towns.

### Modeling highlights
- Fine-tuned ResNet50 and VGG16 to 93% test accuracy with early-stopping on stratified validation folds.
- Added Grad-CAM overlays plus confusion-matrix storytelling to verify that Amherst-specific cues (brick façades, Pioneer Valley tree lines, PVTA buses) truly influenced predictions.

### Takeaways
- Urban morphology signals climb quickly with enough diversity in the capture set.
- Interpretability artifacts are essential for communicating why a classification matters to planners and local stakeholders.
