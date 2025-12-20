---
title: "Qingdao Meeting: Real-time GNSS and Seismic Monitoring"
event: "2025 Geodesy and Navigation Comprehensive Academic Annual Conference"
event_url: ''
location: "Qingdao, China"
summary: "Demonstrates an end-side real-time GNSS source location inversion based on PPP-B2b, with representative cases."
date: '2025-05-17T09:00:00+08:00'
publishDate: '2025-11-30T00:00:00+08:00'
date_end: '2025-05-19T17:00:00+08:00'
authors:
  - admin
featured: true
image:
  caption: "Image credit: Qingdao"
  focal_point: Center
  preview_only: false
links:
  - type: poster
    label: "Poster"
    url: uploads/qingdao-poster.pdf
  # - type: custom
  #   label: "News"
  #   url: /#news
projects: []
slides: ''
---

This poster focuses on an end-side integrated solution for real-time GNSS and seismic monitoring, covering:

- Motivation: Leverage GNSS’s non-saturation advantage for rapid displacement/magnitude evaluation
- Data & Corrections: Ingest RTPPP streams and fuse PPP-B2b/precise corrections
- Method: Time-series feature engineering + lightweight models for online detection and estimation
- Experiments & Cases: Multi-station and historical-event evaluation on latency and robustness
- Engineering: Ingestion, cleaning, inference, visualization, and publishing

## Poster Summary
We present an end-side integrated solution for real-time GNSS and seismic monitoring, targeting robust, low-latency source detection and parameter estimation under dynamic streaming scenarios.
- Motivation: Utilize GNSS’s non-saturation advantage for rapid displacement/magnitude evaluation in EEW and post-event assessment.
- Data & Corrections: Ingest RTPPP streams and fuse PPP-B2b/precise corrections to improve stability and timeliness.
- Method: Combine time-series feature engineering with lightweight models to enable on-device online detection and estimation.
- Experiments & Cases: Validate latency, robustness, and cross-event generalization across multiple stations and historical events.
- Engineering: End-to-end pipeline covering ingestion, cleaning, inference, visualization, and result publishing.

## Contributions
- Propose an end-side pipeline for detection/estimation on real-time GNSS streams.
- Demonstrate low latency and robustness across scenarios.
- Provide reusable implementation and deployment notes.

## Workflow Overview
1. Data Ingestion: RTPPP stream + PPP-B2b/precise corrections
2. Preprocessing: quality control, drift/baseline correction, noise suppression
3. Features & Detection: time/frequency features + lightweight detection model
4. Estimation & Correction: source parameter estimation + physics consistency checks
5. Output & Presentation: result delivery, visualization, and uncertainty

## Poster Figure
![Poster illustration](/events/qingdao-meeting/img1.jpg)
