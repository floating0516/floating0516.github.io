---
title: "{{ replace .Name "-" " " | title }}"
event: "Conference or Academic Event Name"
event_url: ''
location: "City, Country / Online"
summary: "One sentence summarizing the activity, presented work, and research topic."
date: '{{ .Date.Format "2006-01-02T15:04:05-07:00" }}'
publishDate: '{{ .Date.Format "2006-01-02T15:04:05-07:00" }}'
date_end: '{{ .Date.Format "2006-01-02T17:00:00-07:00" }}'
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
- Date: Month day–day, year
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
