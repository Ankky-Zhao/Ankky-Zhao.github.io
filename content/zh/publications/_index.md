---
title: 论文
date: '2026-10-20'
type: landing
sections:
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
cascade:
  show_date: false
  show_date_updated: false
  reading_time: false
---
