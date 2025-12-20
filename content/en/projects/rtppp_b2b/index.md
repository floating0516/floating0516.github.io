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

RTPPP_B2b is a C++ library that decodes BeiDou PPP‑B2b broadcasts and exposes precise orbit/clock corrections required for real-time precise point positioning (PPP). It includes stream parsing, buffering, integrity checks, and utilities for seamless integration into GNSS processing pipelines.

<!--more-->
**Use Cases**
- Real-time PPP augmentation and positioning services
- Seismic displacement evaluation and rapid parameter estimation
- GNSS stream decoding and downstream feature computation

**Key Features**
- PPP‑B2b broadcast decoding (precise orbit/clock corrections)
- Stream parsing and buffer management for real-time data
- Integrity checks and anomaly detection for robustness

**Typical Integration Workflow**
1. Ingest B2b broadcast stream
2. Decode and extract precise corrections (orbit/clock)
3. Feed corrections into PPP engine or filters for real-time solutions
4. Output positioning solutions or features for downstream tasks

**Engineering & Reusability**
- Open-source implementation suitable for production and research reuse
