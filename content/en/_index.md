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
      text: ''
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
      title: '📚 My Research'
      subtitle: 'Data-Driven Geodesy'
      text: |-
        My research sits at the intersection of **Real-Time GNSS (RT-GNSS)** and **Artificial Intelligence (AI)**.

        I focus on a core challenge in disaster monitoring: **how to rapidly and reliably detect seismic signals from high-frequency real-time GNSS streams and estimate magnitudes using deep learning?**

        Key directions:
        * **Real-time streaming:** Data cleaning and positioning with real-time precise point positioning (RTPPP) based on Linux, RTKLIB/BNC, with support for BeiDou-3 **PPP-B2b** broadcast corrections for real-time augmentation.
        * **Deep learning modeling:** Hybrid architectures with **CNN** and **Transformer** to extract spatiotemporal features from GNSS time series.
        * **Disaster mitigation:** Low-latency, high-reliability models for **Earthquake Early Warning (EEW)** and magnitude estimation, improving timeliness from a data-driven perspective.

        Collaboration is welcome for AI for Science and geoscience big data.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
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
  - block: collection
    # Removed News section from navbar/menu
---
