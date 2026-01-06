---
layout: page
title: Bearing Fault Classification with Vision Transformers
description: ViT-based condition monitoring pipeline for fine-grained bearing fault diagnosis from vibration signals.
img: assets/img/2.jpg
importance: 4
category: work
github:
---

This project turns 1D vibration signals from rotating machinery into rich 2D time–frequency representations and feeds them into a Vision Transformer-based classifier for **fine-grained bearing fault diagnosis**.

### Approach
- Converted raw vibration traces into spectrogram-style images so ViT could exploit global spatial attention.
- Trained and tuned a ViT backbone to separate **13 bearing defect classes**, including subtle fault modes that look similar in the raw signal.

### Results
- Reached **98.8% accuracy** across 13 classes, demonstrating that transformer-style global context significantly improves reliability over conventional CNN baselines.
- Stress-tested the model under noise and domain shifts to understand when predictions remain trustworthy for real-world predictive maintenance pipelines.


