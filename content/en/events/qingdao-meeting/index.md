---
title: "Qingdao Meeting: Real-time GNSS and Seismic Monitoring"
event: "2025 Geodesy and Navigation Comprehensive Academic Annual Conference"
event_url: ''
location: "Qingdao, China"
summary: "Presents edge-side real-time GNSS source location and parameter estimation with PPP-B2b corrections and representative cases."
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

This poster presents an edge-side processing workflow for real-time GNSS streams in seismic monitoring. It combines RTPPP, PPP-B2b corrections, and lightweight models to support low-latency source detection and parameter estimation under dynamic streaming conditions.

## Poster Summary

Starting from GNSS’s non-saturation advantage in strong-motion displacement observation, the workflow ingests RTPPP streams, fuses PPP-B2b/precise corrections, and performs quality control, feature extraction, online detection, and result publishing. Multi-station and historical-event experiments are used to evaluate latency, robustness, and cross-event generalization.

## Contributions
- Outline an edge-side detection and estimation workflow for real-time GNSS streams.
- Evaluate the feasibility and stability of low-latency processing across multi-station and historical-event scenarios.
- Summarize reusable engineering practices for ingestion, cleaning, inference, visualization, and result delivery.

## Workflow Overview
1. Data Ingestion: RTPPP stream + PPP-B2b/precise corrections
2. Preprocessing: quality control, drift/baseline correction, noise suppression
3. Features & Detection: time/frequency features + lightweight detection model
4. Estimation & Correction: source parameter estimation + physics consistency checks
5. Output & Presentation: result delivery, visualization, and uncertainty

## Poster Figure
![Poster illustration](/events/qingdao-meeting/img1.jpg)
