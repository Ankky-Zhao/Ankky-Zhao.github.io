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
    interests_text: 我关注能够对地理空间进行推理的人工智能系统，如何被构建、被检验并值得信任。当前的工作主要围绕大语言模型与多模态智能体展开，研究它们在分析地理空间模型时如何规划任务、调用工具并核验自身结果，以及如何向不同背景的人解释这些模型。与之相关的另一个问题是，解释能否真实反映模型所依赖的因素，我借助真值已知的受控实验来研究这一点。随着多模态模型能够从人们分享的图片和文字中推断其所在位置，位置隐私也成为我日益关注的方向。
    headings:
      about: 个人简介
      education: 教育背景
      interests: 研究兴趣
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
    title: 论文
    subtitle: 已发表的同行评审论文，附框架图与公开代码<br><span style="display:inline-flex;gap:.6rem;margin-top:1rem;flex-wrap:wrap;justify-content:center"><a href="https://scholar.google.com/citations?user=R5_5OiwAAAAJ&hl=en" target="_blank" rel="noopener" class="inline-flex items-center gap-2 px-4 h-10 rounded-full bg-white dark:bg-gray-800 text-gray-700 dark:text-gray-200 shadow-sm hover:shadow-md hover:-translate-y-0.5 hover:text-primary-600 dark:hover:text-primary-300 transition-all duration-300 border border-gray-200 dark:border-gray-700 text-sm font-medium"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="currentColor" width="18" height="18" aria-hidden="true"><path d="M12 24a7 7 0 1 1 0-14 7 7 0 0 1 0 14zm0-24L0 9.5l4.838 3.94A8 8 0 0 1 12 9a8 8 0 0 1 7.162 4.44L24 9.5z"/></svg><span>Google Scholar 主页</span></a></span>
    filters:
      folders:
      - publications
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
    title: 项目
    subtitle: GitHub 上的开源项目
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
    title: 动态
    text: |-
      **2026 年 10 月** · 个人主页上线，欢迎在可信人工智能与大语言模型智能体方向开展合作，详见[欢迎合作](/zh/collaborate/)。

      **2026 年 10 月** · 发布 [爬虫学习路线](https://github.com/Ankky-Zhao/web-scraping-roadmap)，从第一个请求到完整爬虫项目的中英双语教程。

      **2026 年 9 月** · 发布 [LLM 智能体学习地图](https://github.com/Ankky-Zhao/llm-agent-roadmap)，涵盖分阶段学习资源与关键论文时间线。

      **2025 年 11 月** · 关于大小语言模型协同抽取地学建模知识的一作论文发表于 *IJGIS*。

      **2025 年 9 月** · 加入慕尼黑工业大学地图学与可视分析教席攻读博士学位。
  design:
    columns: '1'
- block: markdown
  id: teaching
  content:
    title: 教学
    text: |-
      **指导学生** · 指导地理空间 AI 解释评测方向的硕士论文。

      **教学** · 参与慕尼黑工业大学研讨课 *Mapping for a Sustainable World* 的选题设计。曾担任剑桥大学人工智能暑期学校（2021）、武汉大学国际地理信息暑期学校（2022）以及武汉大学《数据结构与程序设计》C++ 课程（2024–2025）助教。
  design:
    columns: '1'
- block: resume-skills
  id: profile
  content:
    title: 技能
    username: me
- block: resume-awards
  id: honours
  content:
    title: 荣誉
    username: me
- block: resume-languages
  id: languages
  content:
    title: 语言
    username: me
- block: markdown
  id: hobbies
  content:
    title: 兴趣爱好
    text: <div style="text-align:center"><span class="inline-block bg-primary-50 dark:bg-gray-800 text-primary-800 dark:text-primary-200 text-base font-medium px-4 py-2 rounded-full border border-primary-200/50 dark:border-primary-800/50 m-1">🏸 羽毛球</span><span class="inline-block bg-primary-50 dark:bg-gray-800 text-primary-800 dark:text-primary-200 text-base font-medium px-4 py-2 rounded-full border border-primary-200/50 dark:border-primary-800/50 m-1">💃 跳舞</span><span class="inline-block bg-primary-50 dark:bg-gray-800 text-primary-800 dark:text-primary-200 text-base font-medium px-4 py-2 rounded-full border border-primary-200/50 dark:border-primary-800/50 m-1">🥾 徒步</span><span class="inline-block bg-primary-50 dark:bg-gray-800 text-primary-800 dark:text-primary-200 text-base font-medium px-4 py-2 rounded-full border border-primary-200/50 dark:border-primary-800/50 m-1">✈️ 旅行</span></div>
  design:
    columns: '1'
- block: collection
  id: blog
  content:
    title: 最新文章
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
      <h2>欢迎合作</h2>
      <p>希望与在<strong>可信与可解释人工智能</strong>、<strong>大语言模型与多模态智能体</strong>（包括智能体的评测、可靠性与推理等前沿问题）以及<strong>人工智能时代的位置隐私</strong>等方向有共同兴趣的研究者合作。贴近 GeoAI 的课题当然欢迎，偏人工智能、把空间数据作为测试场景之一的问题同样欢迎。无论是博士生、博士后还是业界研究人员，合作形式可以是联合论文、数据集或基准，也可以是开源工具。如果你的研究与这些方向有交集，欢迎发邮件简单介绍你正在做的工作。</p>
      <div class="collab-btn"><a href="mailto:anqi.zhao@tum.de?subject=Collaboration">联系我</a></div>
      </div>
  design:
    columns: '1'
---
