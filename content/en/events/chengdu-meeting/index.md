---
title: "GNSS End-Side Source Inversion: Case Studies of 2025 Tibet Dingri Mw 7.1 and Myanmar Mandalay Mw 7.9"
event: "2025 China Geoscience Union Annual Meeting"
event_url: ''
location: "Chengdu, China"
summary: "Demonstrates end-side GNSS source inversion and rapid magnitude estimation based on RTPPP + PPP-B2b, with Dingri Mw 7.1 and Mandalay Mw 7.9 case studies."
date: '2025-10-18T08:00:00+08:00'
publishDate: '2025-11-30T00:00:00+08:00'
date_end: '2025-10-22T17:00:00+08:00'
authors:
  - admin
featured: true
image:
  caption: "Image credit: Conference"
  focal_point: Right
  preview_only: false
links:
  - type: poster
    label: "Poster"
    url: uploads/chengdu-poster.pdf
  - type: custom
    label: "News"
    url: https://faculty.sustech.edu.cn/?p=245743&tagid=chenkj&cat=5&iscss=1&snapid=1&go=2
projects: []
slides: ''
---

This presentation introduces a real-time RTPPP processing pipeline leveraging BeiDou-3 PPP-B2b broadcast corrections, together with CNN/Transformer models for rapid seismic signal detection and magnitude estimation.

## Poster Summary
This poster focuses on end-side GNSS intelligent source inversion. Using the 2025 Tibet Dingri Mw 7.1 and Myanmar Mandalay Mw 7.9 earthquakes as case studies, it demonstrates fast and robust source-parameter estimation from GNSS data in real-time scenarios.

- Motivation: Provide reliable source and magnitude estimates for EEW and rapid assessment without relying on dense networks or offline workflows.
- Data & Processing: Use RTPPP streams and fuse PPP-B2b broadcast corrections to enable continuous, low-latency cleaning and time-series feature extraction.
- Method: Balance physics constraints with data-driven modeling to build an inversion pipeline tailored to GNSS time series, emphasizing robustness and generalization.
- Case Studies: Dingri and Mandalay events demonstrate low-latency source/magnitude estimation and cross-event generalization.
- Engineering: Build an end-to-end workflow for streaming, feature engineering, inference, and visualization to support rapid decisions.

## Contributions
- Propose an end-side GNSS inversion approach to reduce dependencies and improve timeliness.
- Validate feasibility and robustness on real strong earthquakes.
- Provide a reusable engineering pipeline for EEW and rapid assessment.

## Workflow Overview
1. Data Ingestion: RTPPP stream + PPP-B2b corrections
2. Preprocessing: quality control, noise suppression, baseline/drift correction
3. Feature Extraction: source-oriented time/frequency features
4. Estimation & Correction: end-side intelligent inversion + physics consistency checks
5. Output & Visualization: source parameters with uncertainty, result delivery
