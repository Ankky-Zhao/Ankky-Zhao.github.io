---
title: Multi-Agent GeoXAI Architecture
date: '2026-09-01'
summary: A hub-and-spoke multi-agent system that turns attribution outputs of geospatial
  models into interpreted explanations for planners, policymakers and the public.
tags:
- Research
- GeoXAI
- LLM agents
tech_stack:
- Python
- LLM agents
- SHAP
- XGBoost
- GIS
status: In progress
featured: true
weight: 4
links: []
---

Explanations of geospatial machine learning models usually arrive as SHAP values, maps and charts. These outputs are evidence, but most decision makers cannot interpret them on their own, and experts have to redo the interpretation for every new case.

This doctoral project designs an architecture in which a coordinating hub routes each request through specialised agents. One agent clarifies what the user wants to know, one runs the modelling and attribution analysis, one grounds the patterns in geographic and scientific knowledge, one writes the explanation for the intended audience, and one audits the result before delivery. Explanations are layered, moving from data-driven description to geographic mechanism and, for users with decision authority, to actionable context.

The architecture has been tested on population density in Munich and house prices in King County, Washington.

Code will be released after the accompanying manuscript completes peer review.
