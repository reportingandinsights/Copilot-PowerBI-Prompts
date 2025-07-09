---
title: KPI Dashboard Layout
description: “Suggest a high‑level page layout and visual arrangement for a KPI dashboard”
tags: [presentation, ux, dashboard]
version: 1.0
---

**Input Variables**  
- `{{kpis}}` (comma‑separated list)  
- `{{target_audiences}}` (e.g., “operations, analytics”)

**Prompt**  
> “You are a Power BI report designer. For a KPI dashboard tracking  
> `{{kpis}}` intended for `{{target_audiences}}`, suggest a page layout:  
> • Which visuals (cards, gauges, trends) to use for each KPI  
> • Their arrangement and grouping on a single canvas  
> • Any recommended slicers or filters for interactivity”

**Example Usage**  
```bash
copilot invoke --prompt-file prompts/presentation/KPI Dashboard Layout.md \
               --var kpis="Attendance, Baptisms, Giving Churn" \
               --var target_audiences="operations"
