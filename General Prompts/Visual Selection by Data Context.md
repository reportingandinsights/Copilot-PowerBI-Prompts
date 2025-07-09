---
title: Visual Selection by Data Context
description: “Recommend the optimal visual types given columns and analysis goals”
tags: [presentation, ux, visuals]
version: 1.0
---

**Input Variables**  
- `{{columns}}` (e.g., “Date, Attendance, Region”)  
- `{{analysis_goal}}` (e.g., “trend over time”, “geographic comparison”)

**Prompt**  
> “In Power BI, given these fields: `{{columns}}` and the goal to  
> `{{analysis_goal}}`, recommend the best visual types (e.g., line chart, map,  
> stacked bar) and explain why they fit.”

**Example Usage**  
```bash
copilot invoke --prompt-file prompts/presentation/Visual Selection by Data Context.md \
               --var columns="Date, Attendance, Region" \
               --var analysis_goal="geographic comparison"
