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
        text: 下载简历
        url: https://ankky-zhao.github.io/uploads/cv.pdf
      headings:
        about: '个人简介'
        education: '教育背景'
        interests: '研究兴趣'
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
      title: '研究方向'
      subtitle: ''
      text: |-
        地理空间人工智能模型已被用于城市规划、环境监测和政策制定，但其解释大多停留在只有建模专家才能读懂的归因分数上。我的研究把解释视为一个地理信息传达问题。在系统层面，设计基于大语言模型的多智能体架构，分析地理空间模型、将其模式与地理知识相关联，并面向不同受众生成相应的解释。在科学问题层面，借助真值已知的受控实验，检验这些解释是否忠实反映了模型真正依赖的因素。
    design:
      columns: '1'

  - block: portfolio
    id: projects
    content:
      title: '项目'
      subtitle: '研究系统与开源学习资源'
      filters:
        folders:
          - projects
      buttons:
        - name: 全部
          tag: '*'
        - name: 研究
          tag: Research
        - name: 开源
          tag: Open source
      default_button_index: 0
      sort_by: weight
    design:
      columns: 2
      fallback_icon: map

  - block: collection
    id: papers
    content:
      title: '论文'
      text: '完整列表见 [Google Scholar](https://scholar.google.com/citations?user=R5_5OiwAAAAJ&hl=en)。'
      filters:
        folders:
          - publications
    design:
      view: citation

  - block: markdown
    id: news
    content:
      title: '动态'
      text: |-
        **2026 年 10 月** · 发布 [爬虫学习路线](https://github.com/Ankky-Zhao/web-scraping-roadmap)，从第一个请求到完整爬虫项目的中英双语教程。

        **2026 年 9 月** · 发布 [LLM 智能体学习地图](https://github.com/Ankky-Zhao/llm-agent-roadmap)，涵盖分阶段学习资源与关键论文时间线。

        **2025 年 11 月** · 关于大小语言模型协同抽取地学建模知识的一作论文发表于 *IJGIS*。

        **2025 年 9 月** · 加入慕尼黑工业大学地图学与可视分析教席攻读博士学位。
    design:
      columns: '1'

  - block: markdown
    id: teaching
    content:
      title: '教学与学术服务'
      text: |-
        **指导学生** · 指导地理空间 AI 解释评测方向的硕士论文。

        **教学** · 参与慕尼黑工业大学研讨课 *Mapping for a Sustainable World* 的选题设计。曾担任剑桥大学人工智能暑期学校（2021）、武汉大学国际地理信息暑期学校（2022）以及武汉大学《数据结构与程序设计》C++ 课程（2024–2025）助教。

        **审稿** · *Transactions in GIS*、*Geo-spatial Information Science*。
    design:
      columns: '1'

  - block: map
    id: map
    content:
      title: '从武汉到慕尼黑'
      subtitle: '我的地理学之路'
      markers:
        - lat: 30.5360
          lng: 114.3600
          title: 武汉大学
          description: 测绘工程学士、地图学与地理信息系统硕士
        - lat: 48.1497
          lng: 11.5679
          title: 慕尼黑工业大学
          description: 地图学与可视分析教席博士在读
    design:
      layout: map-only
      style: light
      height: sm
      cooperative_gestures: true

  - block: collection
    id: blog
    content:
      title: '最新文章'
      count: 3
      filters:
        folders:
          - blog
      order: desc
    design:
      view: card
---
