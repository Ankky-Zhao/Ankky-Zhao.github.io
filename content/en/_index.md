---
title: ''
summary: ''
date: 2026-10-19
type: landing

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: Download CV
        url: uploads/cv.pdf
      headings:
        about: 'About Me'
        education: ''
        interests: ''
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: markdown
    content:
      title: 'Research'
      subtitle: ''
      text: |-
        Geospatial AI models are increasingly used in planning, environmental monitoring and policy, yet their explanations usually stop at attribution scores that only modelling experts can read. My work treats explanation as a geographic communication problem. On the system side, I design LLM-based multi-agent architectures that analyse a geospatial model, ground its patterns in geographic knowledge and deliver explanations tailored to different audiences. On the scientific side, I examine whether those explanations stay faithful to what the model actually relies on, using controlled experiments in which the ground truth is known.
    design:
      columns: '1'

  - block: portfolio
    id: projects
    content:
      title: 'Projects'
      subtitle: 'Research systems and open learning resources'
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
        - name: Research
          tag: Research
        - name: Open source
          tag: Open source
      default_button_index: 0
      sort_by: weight
    design:
      columns: 2
      fallback_icon: map

  - block: collection
    id: papers
    content:
      title: 'Publications'
      text: 'A complete list is available on [Google Scholar](https://scholar.google.com/citations?user=R5_5OiwAAAAJ&hl=en).'
      filters:
        folders:
          - publications
    design:
      view: citation

  - block: markdown
    id: news
    content:
      title: 'News'
      text: |-
        **Oct 2026** · Released the [Web Scraping Roadmap](https://github.com/Ankky-Zhao/web-scraping-roadmap), a bilingual guide from first request to a finished scraping project.

        **Sep 2026** · Released the [LLM Agent Roadmap](https://github.com/Ankky-Zhao/llm-agent-roadmap), an open learning map of LLM agents with curated resources and a key-papers timeline.

        **Nov 2025** · First-author paper on coordinating large and small language models for geoprocessing knowledge extraction published in *IJGIS*.

        **Sep 2025** · Started my PhD at the Chair of Cartography and Visual Analytics, TUM.
    design:
      columns: '1'

  - block: markdown
    id: teaching
    content:
      title: 'Teaching & Service'
      text: |-
        **Supervision** · Master's theses on benchmarking and evaluating explanations of geospatial AI.

        **Teaching** · Topic design for the seminar *Mapping for a Sustainable World*, TUM. Earlier teaching assistant for the Artificial Intelligence Summer School at the University of Cambridge (2021), the International Geoinformatics Summer School (2022) and *Data Structure and Programming* in C++ (2024–2025) at Wuhan University.

        **Reviewing** · *Transactions in GIS*, *Geo-spatial Information Science*.
    design:
      columns: '1'

  - block: map
    id: map
    content:
      title: 'From Wuhan to Munich'
      subtitle: 'Places that shaped my path in geography'
      markers:
        - lat: 30.5360
          lng: 114.3600
          title: Wuhan University
          description: B.Eng. and M.Sc. in geodesy, cartography and GIS
        - lat: 48.1497
          lng: 11.5679
          title: Technical University of Munich
          description: PhD at the Chair of Cartography and Visual Analytics
    design:
      layout: map-only
      style: light
      height: sm
      cooperative_gestures: true

  - block: collection
    id: blog
    content:
      title: 'Recent Posts'
      count: 3
      filters:
        folders:
          - blog
      order: desc
    design:
      view: card
---
