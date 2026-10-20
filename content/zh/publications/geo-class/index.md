---
title: Geo-CLASS：从 Earth Engine 脚本中抽取建模知识
date: '2025-11-03'
summary: 协同大语言模型与小语言模型，从众包的 Google Earth Engine 脚本中抽取可复用的地学处理建模知识。
tags:
- First author
- LLM
- Knowledge graphs
tech_stack:
- LLM + SLM coordination
- Chain-of-thought prompting
- Embedding-based ontology mapping
- Knowledge graphs
status: IJGIS 2026
featured: true
weight: 3
links:
- type: doi
  url: https://doi.org/10.1080/13658816.2025.2577252
  label: 论文
  icon: document-text
- type: code
  url: https://github.com/Ankky-Zhao/Geo-CLASS
  label: 代码
  icon: brands/github
byline: '**Zhao A.**, Gui Z., Liang J., Liu Y., Peng D., Wei W., Hou S., Wu H.'
---

网络上共享的大量 Google Earth Engine 脚本包含了地理空间分析的实践知识，涵盖数据选择、云掩膜、指数计算到结果导出等环节。这些知识分散在代码中，难以复用。

![从众包脚本到地学处理知识图谱](geo-class-concept.jpg)
*从脚本中抽取主题、功能、数据源以及时空范围，构建知识图谱。*

Geo-CLASS 协同大语言模型与小语言模型。在领域模式与模式感知的思维链提示引导下，由大语言模型识别脚本中的实体与关系；再由小语言模型通过语义向量化、余弦相似度与最佳匹配，将自由文本描述映射到地学知识库（GCMD、GeoNames、GEE 数据目录与功能词典），使不同脚本中含义相同、表述不同的描述统一为标准化实体。

在从 295,943 个脚本中选取的 237 个脚本上，相较 Llama-3、GPT-3.5 和 GPT-4o 等大语言模型基线，实体与关系识别准确率分别最多提升 31.9% 和 12.0%。

页首为 Geo-CLASS 框架总览图。图片引自 Zhao et al. (2026), *International Journal of Geographical Information Science*, 40(3), 808–841, [doi:10.1080/13658816.2025.2577252](https://doi.org/10.1080/13658816.2025.2577252)。
