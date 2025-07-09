```markdown
---
title: Month To Date Measure
description: “Create a DAX measure for month‑to‑date aggregation”
tags: [data‑modeling, dax, measures, time‑intelligence]
version: 1.0
---

**Input Variables**  
- `{{table_name}}`  
- `{{date_column}}`  
- `{{value_column}}`

**Prompt**  
> “Write a DAX measure **MTD {{value_column}}** that computes the month‑to‑date  
> sum of `{{value_column}}` in `{{table_name}}`, based on `{{date_column}}`.  
> Ensure it dynamically adjusts as the current filter context changes.”

**Example Usage**  
```bash
copilot invoke --prompt-file prompts/data-modeling/measures/Month To Date Measure.md \
               --var table_name="Giving Amount" \
               --var date_column="Date" \
               --var value_column="Giving Type"
