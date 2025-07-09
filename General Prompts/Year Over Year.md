---
title: Year‑Over‑Year Growth
description: “Generate a DAX measure to compute year‑over‑year percent growth”
tags: [data‑modeling, dax, measures, time‑intelligence]
version: 1.0
---

**Input Variables**  
- `{{table_name}}`  
- `{{date_column}}`  
- `{{value_column}}`

**Prompt**  
> “Write a DAX measure **YOY Growth %** that calculates the percent change  
> of `{{value_column}}` in `{{table_name}}` compared to the same period last year,  
> using `{{date_column}}` for time intelligence. Ensure it handles blanks gracefully.”

**Example Usage**  
```bash
copilot invoke --prompt-file prompts/data-modeling/measures/yoy_growth.md \
               --var table_name="Giving" \
               --var date_column="OrderDate" \
               --var value_column="Revenue"
