---
title: Extraction of geoprocessing modeling knowledge from crowdsourced Google Earth
  Engine scripts by coordinating large and small language models
authors:
- me
- Zhipeng Gui
- Jianyuan Liang
- Yuhang Liu
- Dehua Peng
- Wenzhang Wei
- Shuyang Hou
- Huayi Wu
date: '2026-01-01T00:00:00Z'
publication_types:
- article-journal
publication:
  name: International Journal of Geographical Information Science
  short_name: IJGIS
  volume: '40'
  issue: '3'
  pages: 808–841
peer_reviewed: true
featured: true
hugoblox:
  ids:
    doi: 10.1080/13658816.2025.2577252
projects:
- geo-class
summary: 协同大小语言模型，从众包 Earth Engine 脚本中抽取可复用的地学处理建模知识。
tags:
- Geoprocessing
- Large language model
- Prompt engineering
- Chain of thought
- Ontology mapping
publishDate: '2025-11-03T00:00:00Z'
abstract: The widespread use of online geoinformation platforms, such as Google Earth
  Engine (GEE), has produced numerous scripts. Extracting domain knowledge from these
  crowdsourced scripts supports understanding of geoprocessing workflows. Small Language
  Models (SLMs) are effective for semantic embedding but struggle with complex code;
  Large Language Models (LLMs) can summarize scripts, yet lack consistent geoscience
  terminology to express knowledge. In this paper, we propose Geo-CLASS, a knowledge
  extraction framework for geospatial analysis scripts that coordinates large and
  small language models. Specifically, we designed domain-specific schemas and a schema-aware
  prompt strategy to guide LLMs to generate and associate entity descriptions, and
  employed SLMs to standardize the outputs by mapping these descriptions to a constructed
  geoscience knowledge base. Experiments on 237 GEE scripts, selected from 295,943
  scripts in total, demonstrated that our framework outperformed LLM baselines, including
  Llama-3, GPT-3.5 and GPT-4o. In comparison, the proposed framework improved accuracy
  in recognizing entities and relations by up to 31.9% and 12.0%, respectively. Ablation
  studies and performance analysis further confirmed the effectiveness of key components
  and the robustness of the framework. Geo-CLASS has the potential to enable the construction
  of geoprocessing modeling knowledge graphs, facilitate domain-specific reasoning
  and advance script generation via Retrieval-Augmented Generation (RAG).
---

*International Journal of Geographical Information Science*，40(3)，808–841。2025 年 11 月 3 日在线发表。
