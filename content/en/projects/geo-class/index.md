---
title: 'Geo-CLASS: Knowledge from Earth Engine Scripts'
date: '2025-11-03'
summary: A pipeline that coordinates large and small language models to extract reusable
  geoprocessing modelling knowledge from crowdsourced Google Earth Engine scripts.
tags:
- Research
- Knowledge extraction
- LLM
tech_stack:
- LLM
- Small language models
- Google Earth Engine
- Knowledge graphs
status: Published
featured: true
weight: 3
links:
- type: custom
  url: https://doi.org/10.1080/13658816.2025.2577252
  icon: document-text
  label: Paper
---

Thousands of Google Earth Engine scripts shared online encode practical knowledge about how geospatial analyses are built, from data selection and cloud masking to index calculation and export. This knowledge is scattered across code and hard to reuse.

Geo-CLASS coordinates a large language model with smaller, cheaper models so that the large model handles the reasoning-heavy steps while the small models carry the bulk of routine extraction. The extracted steps and their dependencies are organised as structured modelling knowledge that can support retrieval and reuse.

Published in the *International Journal of Geographical Information Science*, 2026.
