---
# Leave the homepage title empty to use the site title
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
        I am an MSc student in Geophysics in the [Chen Kejie Group](https://faculty.sustech.edu.cn/?tagid=chenkj&iscss=1&snapid=1&orderby=date&go=2) at Southern University of Science and Technology (SUSTech). My research sits at the intersection of artificial intelligence, real-time high-rate GNSS, and seismic hazard monitoring.

        I work on extracting seismic displacement and crustal deformation signals from real-time GNSS streams, using deep learning models such as CNNs and Transformers for low-latency detection and rapid magnitude estimation. Around this goal, I am building research workflows that combine RTPPP, PPP-B2b corrections, stream processing, and reproducible experimentation.

        I aim to connect engineering implementation with geoscience questions, advancing data-driven geodesy for earthquake early warning and disaster mitigation. I welcome collaboration on AI for Science, real-time GNSS, and geoscience big data.
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: 'About'
        education: 'Education'
        interests: 'Interests'
    design:
      css_class: hbx-bg-gradient
      avatar:
        size: medium
        shape: circle
  - block: markdown
    content:
      title: 'My Research'
      subtitle: 'Data-Driven Geodesy'
      text: |-
        My research centers on one question: **how can real-time high-rate GNSS data and deep learning support low-latency earthquake early warning and rapid magnitude estimation?**

        I currently focus on three directions:
        * **Real-time GNSS pipelines:** Stream cleaning, positioning, and quality control with Linux, RTKLIB/BNC, and RTPPP, including BeiDou-3 PPP-B2b broadcast corrections for real-time augmentation.
        * **Geoscience time-series modeling:** CNN, Transformer, and hybrid architectures for extracting spatiotemporal features and post-seismic responses from GNSS displacement series.
        * **Earthquake early warning applications:** Data-driven methods for low-latency detection, rapid magnitude estimation, and uncertainty-aware decision support in disaster mitigation.
    design:
      columns: '1'
  - block: collection
    id: talks
    content:
      title: Academic Activities
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
      title: Selected Projects
      filters:
        folders:
          - projects
    design:
      view: card
      columns: 3
      spacing:
        padding: [0, 0, 0, 0]
---
