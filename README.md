# 2026-AI-Development
Winter 2026 AI Development Training Series

This course was developed in partnership between the University of Chicago's [Career Advancement Office](https://careeradvancement.uchicago.edu/) and the University of Chicago's [Data Science Institute](https://datascience.uchicago.edu/).


## Workshop: AI Development (4-part series)

This repository contains materials for a four-part workshop on AI development for advanced undergraduates (3rd/4th year).

### Lecture 1 (slides-first)
- **Topic**: Foundations
- **Slides**: `lecture_1/slides/lecture_1.pdf`


- **Readings for lecture 2**:
  - **Context Engineering** 
    - [Effective Context Engineering for AI Agents](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents) - Anthropic's guide to designing context windows for reliable agent behavior.
    - [Context Engineering](https://simonwillison.net/2025/Jun/27/context-engineering/) - Simon Willison's take.
    - [Agent Best Practices](https://cursor.com/blog/agent-best-practices) - Cursor's guide to context engineering.

  - [Welcome to Gas Town](https://steve-yegge.medium.com/welcome-to-gas-town-4f25ee16dd04) - LONG, only read as long as you are interested!
  
  - **Gary Marcus on AI Limitations** 
    - [Why ChatGPT Can't Be Trusted With](https://garymarcus.substack.com/p/why-chatgpt-cant-be-trusted-with) - Discussion of reliability issues and when not to trust LLM outputs.
    - [Breaking: Marcus Weighs In, Mostly](https://garymarcus.substack.com/p/breaking-marcus-weighs-in-mostly) - Critical analysis of AI capabilities and limitations.
    - [Let's Be Honest: Generative AI Isn't](https://garymarcus.substack.com/p/lets-be-honest-generative-ai-isnt) - Perspective on what generative AI can and cannot do reliably.
  

## Under Construction below!


### Lecture 2 (HITL + evaluation)
- **Problem**: Marketing automation / outreach drafting with compliance
- **Notebook**: `lecture_2/notebooks/lecture_2_marketing_hitl.ipynb`
- **Data/docs**: `lecture_2/data/` (leads + brand + product one-pager + rubric)

### Lecture 3 (grounding + API actions)
- **Problem**: Support ticket triage with grounded replies and safe external actions
- **Notebook**: `lecture_3/notebooks/lecture_3_support_triage_api.ipynb`
- **Data/docs**: `lecture_3/data/` (tickets + KB + stub API data)

### Lecture 4 (tools/MCP-like + orchestrator)
- **Problem**: Research brief generation using a tool registry and a simple orchestrator loop
- **Notebook**: `lecture_4/notebooks/lecture_4_tooling_orchestrator.ipynb`
- **Data/docs**: `lecture_4/data/` (docs + market signals + tool registry)

## Running notebooks (per lecture)

Each lecture directory contains a `Makefile`, `Dockerfile`, and `pyproject.toml`.

From a lecture directory (e.g. `lecture_2/`):
- `make build`
- `make notebook` (starts Jupyter in Docker on port 8888)
- `make interactive` (drops you into a bash shell in the container)

## Building slides

Slides are in Beamer (LaTeX) under each lecture’s `slides/` folder.

Example:
```bash
cd lecture_1/slides
pdflatex lecture_1.tex
```
