# Activate Copilot functionality in a Power BI environment like the following and input the desired prompt. 
<img width="2502" height="268" alt="Copilot" src="https://github.com/user-attachments/assets/d0784faa-dc7f-45c9-9742-af7a4b300874" />
<img width="1244" height="1386" alt="Prompt Input" src="https://github.com/user-attachments/assets/7e676b95-e738-408b-962c-572888831d78" />

# All prompts are stored in markdown files like the following and are named according to their intended tasks that the prompts will address. 

---
title: Suggested Tables
description: “Identify which tables you need based on business requirements”
tags: [data‑modeling, tables]
version: 1.0
---

**Input Variables**  
- `{{business_context}}`  
- `{{source_systems}}`

**Prompt**  
> “You are a data architect designing a Power BI semantic model for {{business_context}}.  
> Given these source systems: {{source_systems}}, list the top 5 tables you would include,  
> explain each table’s grain, and note any relationships you’d define.”

**Example Usage**  
```shell
copilot invoke --prompt-file prompts/data-modeling/suggested_tables.md \
               --var business_context="retail sales analysis" \
               --var source_systems="ERP, CRM"
