---
# 留空首页标题以使用站点标题
title: ''
date: 2025-11-29
type: landing

design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: admin
      text: |-
        我是南方科技大学（SUSTech）[陈克杰课题组](https://faculty.sustech.edu.cn/?tagid=chenkj&iscss=1&snapid=1&orderby=date&go=2)的一名硕士研究生，目前正致力于探索人工智能与大地测量学（GNSS）的交叉领域。

        我的核心工作是将先进的深度学习架构（如 CNN 和 Transformer）迁移到地学数据分析中。我正在构建一套数据驱动的实时处理系统，旨在从高频 GNSS 流中精准捕捉地壳形变信号，从而提升地震预警与震级预测的时效性。凭借本科扎实的计算机科学背景，我热衷于利用工程化思维解决复杂的科学问题，推动 AI for Science 在防灾减灾领域的落地。

        科研之外，我是一名 Linux 重度用户和开源技术爱好者。我喜欢钻研高效的开发工具，享受用 Python 和 C++ 构建代码的过程，并乐于通过技术写作分享我的探索心得。
      button:
        text: 下载简历
        url: uploads/resume.pdf
      headings:
        about: '关于我'
        education: '教育经历'
        interests: '研究兴趣'
    design:
      css_class: hbx-bg-gradient
      avatar:
        size: medium
        shape: circle
  - block: markdown
    content:
      title: '我的研究'
      subtitle: 'Data-Driven Geodesy'
      text: |-
        我的研究聚焦于实时全球导航卫星系统（RT-GNSS）与人工智能（AI）的交叉前沿。

        当前，我致力于解决地质灾害监测中的核心挑战：**如何利用深度学习技术，从实时高频 GNSS 数据流中，快速且精准地捕捉地震信号并估计震级？**

        我的主要研究工作包括：
        * **实时流处理：** 基于 Linux 环境与 RTKLIB/BNC 的实时精密单点定位（RTPPP）数据流清洗与解算，支持北斗三号 PPP-B2b 广播改正接入与实时增强。
        * **深度学习建模：** 设计基于 CNN 和 Transformer 的混合架构，挖掘 GNSS 时间序列中的时空特征。
        * **防灾减灾应用：** 构建低延迟、高可靠的地震预警（EEW）与震级估计模型，探索从数据驱动视角提升地质灾害预警的时效性。

        欢迎对 AI for Science 及地学大数据感兴趣的同行交流合作！
    design:
      columns: '1'
  - block: collection
    id: talks
    content:
      title: 参加的学术活动
      count: 8
      filters:
        folders:
          - events
        exclude_future: false
        exclude_past: false
        exclude_featured: false
      order: desc
    design:
      view: card
  - block: collection
    id: projects
    content:
      title: 精选项目
      filters:
        folders:
          - projects
    design:
      view: card
      columns: 3
      spacing:
        padding: [0, 0, 0, 0]
---
