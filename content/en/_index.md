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
        url: https://ankky-zhao.github.io/uploads/cv.pdf
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
      title: 'Research Overview'
      subtitle: ''
      text: |-
        My work sits between machine learning and geographic information science. One line of research builds LLM-based multi-agent systems that combine tool use, planning and verification, and applies them to analysing and explaining GeoAI models for different audiences. A second line examines the explanation methods themselves. Controlled experiments with known ground truth make it possible to measure how well feature attributions and LLM-generated explanations recover what a model relies on, and to identify when spatial structure in the data leads them astray. Earlier work extracted structured knowledge from large corpora of geospatial code by coordinating large and small language models.
    design:
      columns: '1'

  - block: portfolio
    id: research
    content:
      title: 'Research'
      subtitle: 'Published papers, with figures and code where available<br><span style="display:inline-flex;gap:.6rem;margin-top:1rem;flex-wrap:wrap;justify-content:center"><a href="https://scholar.google.com/citations?user=R5_5OiwAAAAJ&hl=en" target="_blank" rel="noopener" class="inline-flex items-center gap-2 px-4 h-10 rounded-full bg-white dark:bg-gray-800 text-gray-700 dark:text-gray-200 shadow-sm hover:shadow-md hover:-translate-y-0.5 hover:text-primary-600 dark:hover:text-primary-300 transition-all duration-300 border border-gray-200 dark:border-gray-700 text-sm font-medium"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" width="18" height="18" aria-hidden="true"><path d="M12 24a7 7 0 1 1 0-14 7 7 0 0 1 0 14zm0-24L0 9.5l4.838 3.94A8 8 0 0 1 12 9a8 8 0 0 1 7.162 4.44L24 9.5z"/></svg><span>Google Scholar profile</span></a><a href="/publications/" class="inline-flex items-center gap-2 px-4 h-10 rounded-full bg-white dark:bg-gray-800 text-gray-700 dark:text-gray-200 shadow-sm hover:shadow-md hover:-translate-y-0.5 hover:text-primary-600 dark:hover:text-primary-300 transition-all duration-300 border border-gray-200 dark:border-gray-700 text-sm font-medium"><span>Full publication list</span></a></span>'
      filters:
        folders:
          - research
      buttons:
        - name: All
          tag: '*'
        - name: First author
          tag: First author
        - name: LLM & agents
          tag: LLM
        - name: Knowledge graphs
          tag: Knowledge graphs
        - name: Spatial data & vision
          tag: Spatial data
      default_button_index: 0
      sort_by: date
      archive:
        enable: false
    design:
      columns: 3
      fallback_icon: document-text

  - block: portfolio
    id: projects
    content:
      title: 'Projects'
      subtitle: 'Open-source projects on GitHub'
      filters:
        folders:
          - projects
      sort_by: weight
      archive:
        enable: false
    design:
      columns: 2
      fallback_icon: code-bracket

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
