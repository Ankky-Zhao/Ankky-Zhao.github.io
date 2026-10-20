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
      title: '研究概述'
      subtitle: ''
      text: |-
        我的研究位于机器学习与地理信息科学之间。一条主线是构建结合工具调用、任务规划与结果核验的多智能体大语言模型系统，用于分析 GeoAI 模型，并面向不同受众解释其行为。另一条主线关注解释方法本身，借助真值已知的受控实验，度量特征归因与大语言模型生成的解释在多大程度上还原了模型真正依赖的因素，并识别数据中的空间结构在哪些情况下会使解释产生偏差。此前的工作则通过协同大小语言模型，从大规模地学代码中抽取结构化知识。
    design:
      columns: '1'

  - block: portfolio
    id: research
    content:
      title: '研究'
      subtitle: '已发表论文，附框架图与公开代码<br><span style="display:inline-flex;gap:.6rem;margin-top:1rem;flex-wrap:wrap;justify-content:center"><a href="https://scholar.google.com/citations?user=R5_5OiwAAAAJ&hl=en" target="_blank" rel="noopener" class="inline-flex items-center gap-2 px-4 h-10 rounded-full bg-white dark:bg-gray-800 text-gray-700 dark:text-gray-200 shadow-sm hover:shadow-md hover:-translate-y-0.5 hover:text-primary-600 dark:hover:text-primary-300 transition-all duration-300 border border-gray-200 dark:border-gray-700 text-sm font-medium"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" width="18" height="18" aria-hidden="true"><path d="M12 24a7 7 0 1 1 0-14 7 7 0 0 1 0 14zm0-24L0 9.5l4.838 3.94A8 8 0 0 1 12 9a8 8 0 0 1 7.162 4.44L24 9.5z"/></svg><span>Google Scholar 主页</span></a><a href="/zh/publications/" class="inline-flex items-center gap-2 px-4 h-10 rounded-full bg-white dark:bg-gray-800 text-gray-700 dark:text-gray-200 shadow-sm hover:shadow-md hover:-translate-y-0.5 hover:text-primary-600 dark:hover:text-primary-300 transition-all duration-300 border border-gray-200 dark:border-gray-700 text-sm font-medium"><span>完整论文列表</span></a></span>'
      filters:
        folders:
          - research
      buttons:
        - name: 全部
          tag: '*'
        - name: 第一作者
          tag: First author
        - name: 大模型与智能体
          tag: LLM
        - name: 知识图谱
          tag: Knowledge graphs
        - name: 时空数据与视觉
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
      title: '项目'
      subtitle: 'GitHub 上的开源项目'
      filters:
        folders:
          - projects
      sort_by: weight
      archive:
        enable: false
    design:
      columns: 2
      fallback_icon: code-bracket

  - block: cta-card
    id: collaborate
    content:
      title: '欢迎合作'
      text: |-
        希望结识在**面向地理空间分析的大语言模型智能体**、**GeoAI 模型的解释与评测**、**地学代码与文本的知识抽取**等方向有共同兴趣的研究者。无论是博士生、博士后还是业界研究人员，合作形式可以是联合论文、数据集或基准，也可以是开源工具。如果你的研究与这些方向有交集，欢迎发邮件简单介绍你正在做的工作。
      button:
        text: '联系我'
        url: 'mailto:anqi.zhao@tum.de?subject=Collaboration'
    design:
      card:
        css_class: 'bg-gradient-to-br from-primary-700 to-secondary-600 text-white shadow-xl'

  - block: markdown
    id: news
    content:
      title: '动态'
      text: |-
        **2026 年 10 月** · 个人主页上线，欢迎在大语言模型智能体与 GeoAI 方向开展合作，详见[欢迎合作](#collaborate)。

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
