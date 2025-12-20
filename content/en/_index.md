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
        I am a master’s student in the [Chen Kejie Group](https://faculty.sustech.edu.cn/?tagid=chenkj&iscss=1&snapid=1&orderby=date&go=2) at Southern University of Science and Technology (SUSTech), exploring the intersection of Artificial Intelligence and Geodesy (GNSS).

        My work focuses on bringing modern deep learning architectures (such as CNNs and Transformers) into geoscience data analysis. I am building a data-driven real-time processing system to capture crustal deformation signals from high-rate GNSS streams, improving the timeliness of earthquake early warning and magnitude estimation. With a solid undergraduate background in computer science, I enjoy solving complex scientific problems with an engineering mindset and advancing AI for Science in disaster mitigation.

        Outside research, I am a Linux power user and open-source enthusiast. I like exploring efficient developer tools, enjoy building with Python and C++, and share my learnings through technical writing.
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
        My research focuses on the intersection of real-time GNSS (RT-GNSS) and Artificial Intelligence (AI).
        
        I work on a key challenge in geohazard monitoring: **how to use deep learning to quickly and accurately detect seismic signals from high-rate real-time GNSS streams and estimate magnitudes?**

        Key directions:
        * **Real-time streaming:** Real-time precise point positioning (RTPPP) data-stream cleaning and processing on Linux with RTKLIB/BNC, supporting BeiDou-3 PPP-B2b broadcast corrections for real-time augmentation.
        * **Deep learning modeling:** Hybrid CNN + Transformer architectures to extract spatiotemporal features from GNSS time series.
        * **Disaster mitigation:** Low-latency, high-reliability models for earthquake early warning (EEW) and rapid magnitude estimation.

        Collaboration is welcome if you are interested in AI for Science or geoscience big data.
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
