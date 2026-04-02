---
name: denario-research
description: "Run scientific research workflows using Denario MCP tools — from data analysis to paper generation."
user-invocable: true
---

# Denario Research

Run scientific research workflows using the Denario MCP server.

## When to Use

- "Research dark energy constraints"
- "Analyze this dataset"
- "Generate a research idea about CMB lensing"
- "Write a paper on my results"
- "Evaluate my analysis"
- "What methods should I use for X?"

## How It Works

Denario provides a full research pipeline via MCP tools. Use them individually or as a sequence:

1. **Setup** — `denario_setup` to initialize a project with a topic and dataset
2. **EDA** — `denario_eda` to explore the data, find patterns, generate summary statistics
3. **Idea** — `denario_idea` to generate a research hypothesis or question
4. **Methods** — `denario_methods` to design the methodology
5. **Results** — `denario_results` to run the analysis
6. **Evaluate** — `denario_evaluate` to assess quality and robustness
7. **Paper** — `denario_paper` to draft a scientific paper

Not every task needs the full pipeline. Use individual tools for targeted requests:
- Quick brainstorm → `denario_idea`
- Data exploration → `denario_eda`
- Check results quality → `denario_evaluate`

## Usage

```
/denario-research [topic or task description]
```

Examples:
```
/denario-research CMB lensing constraints from Planck data
/denario-research evaluate my latest analysis
/denario-research full pipeline on dark energy equation of state
```

## File Access

- `denario_list_files` — list files in the current research project
- `denario_read_file` — read a specific file from the project

## Output

Save research outputs to `notes/research-{topic}-{date}.md` with tags `[research, denario]`.
For voice delivery, write summaries to `results/research-{ts}.txt`.
