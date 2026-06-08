---
title: 青岛会议：实时 GNSS 与地震监测
event: 大地测量与导航2025综合学术年会
event_url: ''
location: 中国青岛
summary: 展示基于 PPP-B2b 改正的边缘端实时 GNSS 震源定位与参数估计案例。
date: '2025-05-17T09:00:00+08:00'
publishDate: '2025-11-30T00:00:00+08:00'
date_end: '2025-05-19T17:00:00+08:00'
authors:
  - admin
featured: true
image:
  caption: 'Image credit: Qingdao'
  focal_point: Center
  preview_only: false
links:
  - type: poster
    label: 海报
    url: uploads/qingdao-poster.pdf
  # - type: custom
  #   label: 新闻
  #   url: /#news
projects: []
slides: ''
---

本海报聚焦实时 GNSS 数据流在地震监测中的边缘端处理方案，讨论如何结合 RTPPP、PPP-B2b 改正与轻量模型，在动态流式场景下开展低延迟震源检测和参数估计。

## 海报摘要

研究从 GNSS 在强震位移观测中的抗饱和优势出发，构建面向边缘端部署的实时处理流程：接入 RTPPP 数据流，融合 PPP-B2b/精密改正，完成质量控制、特征提取、在线检测与结果发布。多台站和历史事件实验用于评估流程在延迟、鲁棒性和跨事件泛化方面的表现。

## 主要贡献
- 梳理面向实时 GNSS 流的边缘端检测与估计流程。
- 在多台站和历史事件场景中评估低延迟处理的可行性与稳定性。
- 总结数据接入、清洗、推理、可视化与结果发布中的可复用工程要点。

## 方法流程概览
1. 数据接入：RTPPP 实时流 + PPP-B2b/精密改正
2. 预处理：质量控制、漂移/基线修正、噪声抑制
3. 特征与检测：时序/频域特征 + 轻量检测模型
4. 估计与校正：震源参数估计 + 物理一致性校正
5. 输出与展示：结果推送、可视化与不确定性

## 海报图
![海报示意图](img1.jpg)
