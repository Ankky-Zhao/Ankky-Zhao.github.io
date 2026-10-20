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
      interests_text: |-
        I am interested in how AI systems that reason about place can be built, checked and trusted. Much of my current work concerns LLM and multimodal agents that plan, call tools and verify their own results when analysing geospatial models, and how such agents can explain those models to people with different backgrounds. A related question is whether an explanation reflects what a model actually relies on, which I study with controlled experiments where the ground truth is known. I am also increasingly interested in location privacy, as multimodal models become able to infer where people are from the images and text they share.
      headings:
        about: 'About Me'
        education: ''
        interests: 'Research Interests'
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle

  - block: portfolio
    id: publications
    content:
      title: 'Publications'
      subtitle: 'Peer-reviewed papers, with figures and code where available<br><span style="display:inline-flex;gap:.6rem;margin-top:1rem;flex-wrap:wrap;justify-content:center"><a href="https://scholar.google.com/citations?user=R5_5OiwAAAAJ&hl=en" target="_blank" rel="noopener" class="inline-flex items-center gap-2 px-4 h-10 rounded-full bg-white dark:bg-gray-800 text-gray-700 dark:text-gray-200 shadow-sm hover:shadow-md hover:-translate-y-0.5 hover:text-primary-600 dark:hover:text-primary-300 transition-all duration-300 border border-gray-200 dark:border-gray-700 text-sm font-medium"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" width="18" height="18" aria-hidden="true"><path d="M12 24a7 7 0 1 1 0-14 7 7 0 0 1 0 14zm0-24L0 9.5l4.838 3.94A8 8 0 0 1 12 9a8 8 0 0 1 7.162 4.44L24 9.5z"/></svg><span>Google Scholar profile</span></a></span>'
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
        **Oct 2026** · Launched this website. I am open to collaboration on trustworthy AI and LLM agents, see [Open to Collaboration](#collaborate).

        **Oct 2026** · Released the [Web Scraping Roadmap](https://github.com/Ankky-Zhao/web-scraping-roadmap), a bilingual guide from first request to a finished scraping project.

        **Sep 2026** · Released the [LLM Agent Roadmap](https://github.com/Ankky-Zhao/llm-agent-roadmap), an open learning map of LLM agents with curated resources and a key-papers timeline.

        **Nov 2025** · First-author paper on coordinating large and small language models for geoprocessing knowledge extraction published in *IJGIS*.

        **Sep 2025** · Started my PhD at the Chair of Cartography and Visual Analytics, TUM.
    design:
      columns: '1'

  - block: markdown
    id: teaching
    content:
      title: 'Teaching'
      text: |-
        **Supervision** · Master's theses on benchmarking and evaluating explanations of geospatial AI.

        **Teaching** · Topic design for the seminar *Mapping for a Sustainable World*, TUM. Earlier teaching assistant for the Artificial Intelligence Summer School at the University of Cambridge (2021), the International Geoinformatics Summer School (2022) and *Data Structure and Programming* in C++ (2024–2025) at Wuhan University.
    design:
      columns: '1'

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

  - block: markdown
    id: collaborate
    content:
      title: ''
      text: |-
        <div class="collab-card">
        <h2>Open to Collaboration</h2>
        <p>I would like to work with people who share an interest in <strong>trustworthy and explainable AI</strong>, <strong>LLM and multimodal agents</strong> and newer agent topics such as evaluation, reliability and reasoning, or <strong>location privacy in the age of AI</strong>. Projects close to GeoAI are welcome, and so are questions from the broader AI side where spatial data is one testbed among others. PhD students, postdocs and industry researchers are all welcome, for a joint paper, a dataset or benchmark, or an open-source tool. If this overlaps with your work, a short email about what you are working on is the best way to start.</p>
        <div class="collab-btn"><a href="mailto:anqi.zhao@tum.de?subject=Collaboration">Get in touch</a></div>
        </div>
    design:
      columns: '1'
---
