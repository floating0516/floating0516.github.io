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
  - 开源
image:
  caption: 'RTPPP_B2b 封面'
  focal_point: Center
  preview_only: false
---


RTPPP_B2b 是一个面向北斗 PPP‑B2b 广播改正的 C++ 解码库，用于为实时精密单点定位（PPP）提供精密轨道与钟差改正。它关注从广播数据接入、流式解析到改正量输出的关键环节，为实时 GNSS 解算和下游地震位移分析提供可复用的数据基础设施。

<!--more-->
**适用场景**
- 实时 PPP 增强与高率 GNSS 数据处理
- 地震位移分析与快速参数估计前处理
- GNSS 数据流解码、质量控制与下游特征计算

**核心特性**
- PPP‑B2b 广播解码，提取精密轨道与钟差改正
- 面向实时数据流的解析、缓冲和状态管理
- 完整性校验与异常检测，提升连续处理稳定性

**典型集成流程**
1. 接入 B2b 广播数据流
2. 解码并提取精密轨道/钟差改正
3. 将改正量注入 PPP 引擎或滤波器进行实时解算
4. 输出位置解或下游地震监测任务所需特征

**工程与复用**
- 开源实现，适合用于实时 GNSS 处理管线、科研原型验证和后续工程复用
