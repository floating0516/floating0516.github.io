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
        我是南方科技大学（SUSTech）[陈克杰课题组](https://faculty.sustech.edu.cn/?tagid=chenkj&iscss=1&snapid=1&orderby=date&go=2)的地球物理方向硕士研究生，研究兴趣位于人工智能、实时高率 GNSS 与地震灾害监测的交叉处。

        我的工作关注如何从实时 GNSS 数据流中提取地震位移与地壳形变信号，并结合 CNN、Transformer 等深度学习模型开展低延迟检测与快速震级估计。围绕这一目标，我也在构建 RTPPP、PPP-B2b 改正接入、流式数据处理与可复现实验相结合的研究管线。

        我希望把扎实的工程实现能力与地学问题结合起来，推动数据驱动大地测量方法在地震预警和防灾减灾场景中的应用。欢迎对 AI for Science、实时 GNSS 和地学大数据感兴趣的同行交流合作。
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
        我的研究围绕一个核心问题展开：**如何利用实时高率 GNSS 数据和深度学习方法，为地震预警与快速震级估计提供低延迟、可复现的技术支撑？**

        目前主要关注三个方向：
        * **实时 GNSS 数据链路：** 基于 Linux、RTKLIB/BNC 与 RTPPP 的流式数据清洗、解算和质量控制，并接入北斗三号 PPP-B2b 广播改正实现实时增强。
        * **地学时间序列建模：** 设计 CNN、Transformer 及其混合架构，提取 GNSS 位移序列中的时空特征与震后响应信息。
        * **地震预警应用：** 面向低延迟检测、快速震级估计和不确定性表达，探索数据驱动方法在防灾减灾中的可靠应用。
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
