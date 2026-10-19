---
title: 'Geo-CLASS: Knowledge from Earth Engine Scripts'
date: '2025-11-03'
summary: A pipeline that coordinates large and small language models to extract reusable
  geoprocessing modelling knowledge from crowdsourced Google Earth Engine scripts.
tags:
- Research
- LLM
- Knowledge extraction
tech_stack:
- LLM + SLM coordination
- Chain-of-thought prompting
- Embedding-based ontology mapping
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

![From crowdsourced scripts to a geoprocessing knowledge graph](geo-class-concept.jpg)
*Extracting themes, functions, data sources and spatial and temporal scopes from a script into a knowledge graph.*

Geo-CLASS coordinates a large language model with small language models. Guided by a domain schema and a schema-aware, chain-of-thought prompt, the LLM recognises entities and relations in each script. The SLMs then map the free-text descriptions onto a geoscience knowledge base (GCMD, GeoNames, the GEE data catalogue and a functional dictionary) through semantic vectorisation, cosine similarity and best-match selection, so that synonymous descriptions from different scripts end up as the same standardised entity.

On 237 scripts sampled from 295,943, the framework improved entity and relation recognition accuracy by up to 31.9% and 12.0% over LLM baselines including Llama-3, GPT-3.5 and GPT-4o.

The overview figure at the top shows the full Geo-CLASS framework. Figures from Zhao et al. (2026), *International Journal of Geographical Information Science*, 40(3), 808–841, [doi:10.1080/13658816.2025.2577252](https://doi.org/10.1080/13658816.2025.2577252).
