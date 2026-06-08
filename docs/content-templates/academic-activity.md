# 学术活动内容模板

本模板用于后续补充首页「参加的学术活动 / Academic Activities」卡片内容。当前站点的学术活动由首页 collection 区块读取 `events` 文件夹生成：

- 中文：`content/zh/events/<activity-slug>/index.md`
- 英文：`content/en/events/<activity-slug>/index.md`

建议中英文使用相同的 `<activity-slug>`，方便维护双语内容。例如：

```text
content/zh/events/2026-wuhan-gnss-meeting/index.md
content/en/events/2026-wuhan-gnss-meeting/index.md
```

---

## 中文模板

将下面内容复制到：`content/zh/events/<activity-slug>/index.md`

```markdown
---
title: 活动报告或海报题目
event: 会议或学术活动名称
event_url: ''
location: 中国城市 / 线上
summary: 用一句话概括本次活动、展示内容与研究主题。
date: '2026-01-01T09:00:00+08:00'
publishDate: '2026-01-01T00:00:00+08:00'
date_end: '2026-01-03T17:00:00+08:00'
authors:
  - admin
featured: true
image:
  caption: 'Image credit: 会议现场 / 主办方 / 自摄'
  focal_point: Center
  preview_only: false
links:
  - type: poster
    label: 海报
    url: uploads/example-poster.pdf
  # - type: custom
  #   label: 新闻
  #   url: https://example.com/news
projects: []
slides: ''
---

本次学术活动中，我围绕「研究主题」展示了「方法 / 系统 / 实验结果」的阶段性进展，并与相关领域的老师和同学进行了交流。

## 活动概况

- 活动名称：会议或学术活动名称
- 时间：2026 年 1 月 1 日至 1 月 3 日
- 地点：中国城市 / 线上
- 展示形式：口头报告 / 海报展示 / 邀请报告 / 参会交流
- 主题方向：GNSS、地震监测、AI for Science、实时数据处理等

## 内容摘要

本次展示聚焦于「一句话研究问题」。主要内容包括：

- 研究动机：说明为什么这个问题重要，以及它面向的科学或工程场景。
- 数据与方法：说明使用的数据来源、处理流程、模型或分析方法。
- 实验与案例：概括关键实验设置、案例事件或对比结果。
- 主要结论：用 1–2 条要点总结展示得到的阶段性认识。
- 后续计划：说明下一步准备完善的方向。

## 主要收获

- 与同行交流了「具体问题或方向」。
- 收到关于「方法、实验、展示或应用」的反馈。
- 明确了后续需要补充的实验、数据或分析。

## 相关材料

- 海报 / 幻灯片：见页面上方链接。
- 新闻或会议页面：如有可在 front matter 的 `links` 中补充。
```

---

## English Template

Copy the following content to: `content/en/events/<activity-slug>/index.md`

```markdown
---
title: "Presentation or Poster Title"
event: "Conference or Academic Event Name"
event_url: ''
location: "City, Country / Online"
summary: "One sentence summarizing the activity, presented work, and research topic."
date: '2026-01-01T09:00:00+08:00'
publishDate: '2026-01-01T00:00:00+08:00'
date_end: '2026-01-03T17:00:00+08:00'
authors:
  - admin
featured: true
image:
  caption: "Image credit: Conference / Organizer / Photo by author"
  focal_point: Center
  preview_only: false
links:
  - type: poster
    label: "Poster"
    url: uploads/example-poster.pdf
  # - type: custom
  #   label: "News"
  #   url: https://example.com/news
projects: []
slides: ''
---

At this academic event, I presented recent progress on "research topic", focusing on "method / system / experimental results", and discussed the work with researchers and students in related fields.

## Event Overview

- Event: Conference or academic event name
- Date: January 1–3, 2026
- Location: City, Country / Online
- Format: Oral presentation / poster presentation / invited talk / conference participation
- Topics: GNSS, seismic monitoring, AI for Science, real-time data processing, etc.

## Summary

This presentation focused on "one-sentence research question". The main points include:

- Motivation: Explain why the problem matters and which scientific or engineering scenario it targets.
- Data & Methods: Describe the data source, processing pipeline, model, or analysis method.
- Experiments & Cases: Summarize key experimental settings, case studies, or comparisons.
- Key Findings: Highlight 1–2 main findings or current insights.
- Next Steps: Briefly describe planned improvements or follow-up work.

## Takeaways

- Discussed "specific question or direction" with colleagues.
- Received feedback on "method, experiments, presentation, or applications".
- Identified additional experiments, data, or analyses to be completed.

## Related Materials

- Poster / slides: see the links above.
- News or conference page: add it to `links` in the front matter if available.
```

---

## 字段填写说明

- `title`：卡片和详情页标题，建议使用报告/海报题目。
- `event`：会议或活动名称。
- `event_url`：活动官网；没有就保留空字符串 `''`。
- `location`：地点；中文页写中文，英文页写英文。
- `summary`：首页卡片摘要，控制在一两句话内。
- `date` / `date_end`：活动开始和结束时间，格式参考已有内容。
- `publishDate`：页面发布时间；通常可设为活动开始日或内容整理日期。
- `authors`：个人主页内容保持 `admin`。
- `featured`：设为 `true` 会正常参与首页 collection 展示。
- `image.caption`：没有图片时也可以保留；如添加图片，放在同一活动目录中并按 Hugo Blox 规则引用。
- `links`：常用 `poster`、`slides` 或 `custom`。没有材料时可以设为 `links: []`。
- `projects`：如关联项目，可填项目 slug；没有就保留 `[]`。
- `slides`：如使用 Hugo slides，可填写对应 slug；否则保留空字符串。

## 新增活动检查清单

- [ ] 中文页面已创建：`content/zh/events/<activity-slug>/index.md`
- [ ] 英文页面已创建：`content/en/events/<activity-slug>/index.md`
- [ ] 中英文 `date`、`date_end`、`publishDate` 一致
- [ ] 首页 collection 的 `count: 8` 足够展示新增活动；如活动超过 8 条，可在 `content/zh/_index.md`、`content/en/_index.md` 和 `content/_index.md` 中调整
- [ ] 海报、图片或附件链接可访问
- [ ] 运行 `pnpm build` 确认 Hugo 构建通过
