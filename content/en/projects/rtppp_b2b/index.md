---
title: RTPPP_B2b
date: 2023-10-26
links:
  - type: site
    url: https://github.com/floating0516/RTPPP_B2b
tags:
  - C++
  - GNSS
  - PPP-B2b
  - BeiDou
  - Open Source
image:
  caption: 'RTPPP_B2b cover'
  focal_point: Center
  preview_only: false
---

RTPPP_B2b is a C++ decoder for BeiDou PPP‑B2b broadcast corrections, providing precise orbit and clock corrections for real-time precise point positioning (PPP). It focuses on the key steps from broadcast ingestion and stream parsing to correction output, serving as reusable data infrastructure for real-time GNSS processing and downstream seismic displacement analysis.

<!--more-->
**Use Cases**
- Real-time PPP augmentation and high-rate GNSS data processing
- Preprocessing for seismic displacement analysis and rapid parameter estimation
- GNSS stream decoding, quality control, and downstream feature computation

**Key Features**
- PPP‑B2b broadcast decoding for precise orbit and clock corrections
- Stream parsing, buffering, and state management for real-time data
- Integrity checks and anomaly detection for stable continuous processing

**Typical Integration Workflow**
1. Ingest B2b broadcast streams
2. Decode and extract precise orbit/clock corrections
3. Feed corrections into a PPP engine or filter for real-time positioning
4. Output positioning solutions or features for downstream seismic monitoring tasks

**Engineering & Reusability**
- Open-source implementation designed for real-time GNSS pipelines, research prototyping, and engineering reuse
