---
title: Calculate Running Total
description: “Generate a DAX calculated column for a running total by date”
tags: [data‑modeling, dax]
version: 1.0
---

**Input Variables**  
- `{{table_name}}`  
- `{{date_column}}`  
- `{{value_column}}`

**Prompt**  
> “In Power BI, write a DAX calculated column that computes the running total of  
> `{{value_column}}` in the `{{table_name}}` table, ordered by `{{date_column}}`.  
> Ensure the calculation resets for each fiscal year.”

**Example Usage**  
```bash
copilot invoke --prompt-file prompts/data-modeling/calculated_columns.md \
               --var table_name="Giving" \
               --var date_column="Date" \
               --var value_column="Revenue"
