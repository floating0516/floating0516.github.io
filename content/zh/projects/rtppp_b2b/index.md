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


RTPPP_B2b 是一个用于解码北斗 PPP‑B2b 广播并提供实时精密点位（PPP）所需精密轨道/钟差改正的 C++ 库，包含流式解析、缓冲、完整性校验与便于集成到 GNSS 处理管线的实用工具。

<!--more-->
**适用场景**
- 实时 PPP 增强与定位服务
- 地震位移评估与快速参数估计
- GNSS 数据流解码与下游特征计算

**核心特性**
- PPP‑B2b 广播解码（精密轨道/钟差改正）
- 流式解析与缓冲管理，面向实时数据
- 完整性校验与异常检测，提升稳定性

**典型集成流程**
1. 接入 B2b 广播数据流
2. 解码并提取精密改正（轨道/钟差）
3. 注入 PPP 引擎或滤波器进行实时解算
4. 输出位置解或下游任务所需特征

**工程与复用**
- 开源实现，适合工程落地与科研复用
