---
title: License Plate Recognition Model
category: Research
order: 1
summary: Training and deploying a CNN-based license plate detector tailored for Dubai roads, from dataset curation to ONNX edge inference.
timeline: Jan 2025 – Present
role: Lead Machine Learning Researcher
location: American University in Dubai
skills:
  - PyTorch
  - Computer Vision
  - ONNX Runtime
  - Data Engineering
lead: Building a region-aware perception stack that can power smart parking and campus safety tools without sending data to the cloud.
---

## Overview
I partnered with the American University in Dubai to design a license plate recognition system that reflects the quirks of Gulf roadways. The project began as a way to support campus parking logistics and quickly evolved into a full perception pipeline—from data collection to inference.

The first three months were dedicated to field work: photographing vehicles in varying lighting conditions, angles, and license plate types. I built a dataset of more than 500 annotated Dubai plates, then augmented it with synthetic glare, sand, and occlusion patterns to mimic real-world variability. Each annotation pass is version-controlled so students joining the lab can trace improvements over time.

## Highlights
- **Adaptive training loop:** Designed a PyTorch pipeline with Hydra configuration, cosine learning-rate schedules, and automated hyperparameter sweeps. The detector currently reaches a 0.92 F1-score at IoU 0.5 on a hold-out validation set representing six Emirate plate styles.
- **Edge-friendly deployment:** Exported the trained model to ONNX and profiled it across NVIDIA Jetson Nano, Apple M-series, and CPU-only edge boxes. INT8 dynamic quantization trimmed inference latency by 38% without compromising recall.
- **Human-in-the-loop labeling:** Built a lightweight review tool with Streamlit to let security officers flag misreads and prioritize new data captures. Feedback flows back into the active-learning loop each sprint.

## Impact
The prototype now powers a dashboard that surfaces plate detections in under 120 ms, allowing campus security to follow parking trends in real time. Beyond the university, the dataset and tooling are being reused by Logic Labs students who are learning about embedded vision and sensor fusion.

## What's next
I am integrating plate tracking into a multi-camera setup and experimenting with transformer-based OCR heads to better handle stylized Arabic typography. The next phase also explores privacy-preserving blurring so community deployments remain transparent and trustworthy.
