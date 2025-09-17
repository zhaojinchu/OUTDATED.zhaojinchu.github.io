---
title: Evaluating NPUs vs. Traditional Processors
category: Research
order: 4
summary: Benchmarked neural processing units against CPU/GPU pipelines for edge inference, analyzing performance-per-watt and memory bandwidth trade-offs.
timeline: Jul 2024 – Jan 2025
role: Research Author & Hardware Analyst
location: Dubai College
skills:
  - Benchmarking
  - Embedded Systems
  - Data Visualization
  - Technical Writing
lead: Helping educators and student founders choose the right silicon for AI workloads by pairing quantitative benchmarks with narrative explainers.
---

## Motivation
As Logic Labs students explored AI on microcontrollers, we kept asking which processors could sustain low-latency inference without huge batteries. I turned the question into a formal thesis comparing emerging Neural Processing Units (NPUs) with tuned CPU/GPU baselines across computer vision and speech tasks.

## Experiment design
- Built reproducible benchmarking harnesses in Python, capturing throughput, latency, power draw, and thermal throttling behaviour.
- Tested Qualcomm Hexagon NPUs, Apple Neural Engine, NVIDIA Jetson modules, and ARM Cortex-A series CPUs with quantized MobileNet and Whisper models.
- Instrumented each run with onboard sensors and external power meters to validate vendor-reported specifications.

## Findings
- **Performance-per-watt wins:** Dedicated NPUs delivered up to 3.7× better performance-per-watt on transformer inference compared with CPU-only baselines.
- **Bandwidth bottlenecks:** Memory bandwidth caps often erased theoretical gains; carefully batching workloads on the Jetson Xavier produced more stable latencies than naive streaming.
- **Deployment guidance:** Documented decision trees that educators now use to match project requirements with silicon capabilities, cutting prototyping time by weeks.

## Deliverables
The 6,000-word thesis compiles detailed charts, configuration files, and tuning scripts that continue to guide Logic Labs cohorts. The work now anchors a workshop on hardware-aware AI deployment for regional robotics clubs.
