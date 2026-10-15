# [Project Title: Insert Your Research Topic Here]

> **Student Research Project Template**  
> Course: `[Course ID / Name]` | Institution: `[University / Department]`

---

## 📌 Overview
- **Topic:** `[Brief 1-sentence description of the research topic]`
- **Advisor:** `[Advisor Name]`
- **Team:** `[Student 1]`, `[Student 2]`, `[Student 3]` (See [research-metadata.md](file:///f:/thinkprompt/code/researches/project-research-template/research-metadata.md))
- **Objective:** `[What are you building or investigating?]`

---

## 📂 Project Structure

| File / Folder | Purpose |
| :--- | :--- |
| **[research-metadata.md](file:///f:/thinkprompt/code/researches/project-research-template/research-metadata.md)** | Topic, course, team members, supervisor, milestones |
| **[research-methodology.md](file:///f:/thinkprompt/code/researches/project-research-template/research-methodology.md)** | Problem formulation, approach, dataset, metrics |
| **[literature-review/](file:///f:/thinkprompt/code/researches/project-research-template/literature-review/)** | Survey of related papers, matrix, and research gaps |
| **`research/`** | Experiment plans (`experiment-design.md`), code, and results |
| **`essay-template/`** | Final paper template and report guidelines |

---

## 🧭 Workflow Guide

1. **Step 1:** Fill in team and course information in [research-metadata.md](file:///f:/thinkprompt/code/researches/project-research-template/research-metadata.md).
2. **Step 2:** Summarize existing papers in [literature-review/README.md](file:///f:/thinkprompt/code/researches/project-research-template/literature-review/README.md).
3. **Step 3:** Define your approach, datasets, and baselines in [research-methodology.md](file:///f:/thinkprompt/code/researches/project-research-template/research-methodology.md).
4. **Step 4:** Implement code in `research/experiment-code/` and log findings in `research/experiment-result.md`.
5. **Step 5:** Write your final report following the template in `essay-template/`.

---

## 🚀 Quickstart

```bash
# 1. Set up virtual environment
python -m venv .venv
# Windows:
.venv\Scripts\activate
# Linux/macOS:
source .venv/bin/activate

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run baseline or experiments
python research/experiment-code/main.py
```
