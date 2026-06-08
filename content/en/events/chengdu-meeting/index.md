---
title: "Edge-Side GNSS Source Inversion: Case Studies of the 2025 Tibet Dingri Mw 7.1 and Myanmar Mandalay Mw 7.9 Earthquakes"
event: "2025 China Geoscience Union Annual Meeting"
event_url: ''
location: "Chengdu, China"
summary: "Presents edge-side GNSS source inversion and rapid magnitude estimation using RTPPP and PPP-B2b, with Dingri Mw 7.1 and Mandalay Mw 7.9 case studies."
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

This presentation introduces a real-time precise point positioning (RTPPP) processing pipeline using BeiDou-3 PPP-B2b broadcast corrections. With the 2025 Tibet Dingri Mw 7.1 and Myanmar Mandalay Mw 7.9 earthquakes as case studies, it discusses how GNSS displacement series can support rapid source inversion and magnitude estimation.

## Poster Summary

The poster focuses on edge-side GNSS intelligent source inversion. In real-time scenarios, the workflow ingests RTPPP streams, fuses PPP-B2b broadcast corrections, and performs low-latency cleaning, time-series feature extraction, model inference, and visualization. The Dingri and Mandalay events are used to evaluate feasibility, stability, and cross-event applicability on real strong-earthquake cases.

## Contributions
- Explore an edge-side source inversion workflow for GNSS displacement series, reducing dependence on offline processing chains.
- Evaluate the feasibility and robustness of rapid source/magnitude estimation on two strong-earthquake cases.
- Provide an engineering pipeline for real-time streams, feature engineering, inference, and visualization to support EEW and rapid post-event assessment.

## Workflow Overview
1. Data Ingestion: RTPPP stream + PPP-B2b corrections
2. Preprocessing: quality control, noise suppression, baseline/drift correction
3. Feature Extraction: source-oriented time/frequency features
4. Estimation & Correction: edge-side intelligent inversion + physics consistency checks
5. Output & Visualization: source parameters with uncertainty, result delivery
