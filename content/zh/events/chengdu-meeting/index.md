---
title: GNSS 边缘端震源智能反演：以 2025 年西藏定日 Mw 7.1 和缅甸曼德勒 Mw 7.9 地震为例
event: 2025年中国地球科学联合学术年会
event_url: ''
location: 中国成都
summary: 以定日 Mw 7.1 与曼德勒 Mw 7.9 案例，展示基于 RTPPP 与 PPP-B2b 的 GNSS 边缘端震源反演和快速震级估计。
date: '2025-10-18T08:00:00+08:00'
publishDate: '2025-11-30T00:00:00+08:00'
date_end: '2025-10-22T17:00:00+08:00'
authors:
  - admin
featured: true
image:
  caption: 'Image credit: 会议现场'
  focal_point: Right
  preview_only: false
links:
  - type: poster
    label: 海报
    url: uploads/chengdu-poster.pdf
  - type: custom
    label: 新闻
    url: https://faculty.sustech.edu.cn/?p=245743&tagid=chenkj&cat=5&iscss=1&snapid=1&go=2
projects: []
slides: ''
---

本次分享介绍了基于北斗三号 PPP-B2b 广播改正的实时精密单点定位（RTPPP）数据流处理流程，并以 2025 年西藏定日 Mw 7.1 与缅甸曼德勒 Mw 7.9 地震为案例，讨论 GNSS 位移序列在快速震源反演和震级估计中的应用。

## 海报摘要

海报聚焦 GNSS 边缘端震源智能反演：在实时场景中接入 RTPPP 数据流，融合 PPP-B2b 广播改正，完成低延迟数据清洗、时序特征提取、模型推理与结果可视化。定日和曼德勒两次强震案例用于检验该流程在真实事件中的可行性、稳定性和跨事件适用性。

## 主要贡献

- 探索面向 GNSS 位移序列的边缘端震源反演流程，减少对离线处理链路的依赖。
- 在两次强震案例中评估快速震源/震级估计的可行性与稳健性。
- 给出围绕实时流、特征工程、推理和可视化的工程化管线，为地震预警与震后快速评估提供参考。

## 方法流程概览

1. 数据接入：RTPPP 实时流 + PPP-B2b 改正
2. 预处理：质量控制、噪声抑制、基线/漂移修正
3. 特征提取：面向震源的时序与频域特征
4. 估计与校正：边缘端智能反演 + 物理一致性校正
5. 输出与可视化：震源参数与不确定性评估、结果推送
