---
layout: page
title: SSORT — Semantic Segmentation for Off-Road Traversability
description: SegFormer-based perception stack that maps passable terrain for autonomous robots.
img: assets/img/7.jpg
importance: 3
category: work
github: https://github.com/aeyanashraf/SSORT--Semantic-Segmentation-for-Off-Road-Traversibility
---

Safe off-road autonomy needs dense terrain understanding rather than top-line object detection. **SSORT** combines modern semantic segmentation (SegFormer) with lightweight deployment tooling so robots can reason about mud, brush, gravel, and unstructured boundaries in real time.

### Pipeline
- Curated geospatial datasets from drone and rover captures; synchronized with pixel-perfect masks covering traversable vs. hazardous classes.
- Fine-tuned SegFormer via Hugging Face pipelines, augmenting with photometric and texture jitter that mimic harsh field conditions.
- Benchmarked against DeepLab and UNet variants, improving mean IOU and pixel accuracy by ~10% on the held-out terrain suite.

### Deployment + evaluation
- Flask API exposes batched inference plus a metrics dashboard that tracks IOU, pixel accuracy, and per-class F1 over new uploads.
- Added CUDA-based post-processing to flag uncertainty zones so navigation policies can request human review or re-plan.

SSORT makes it possible to quantify how reliable a segmentation policy is before we trust it on expensive autonomous platforms.
