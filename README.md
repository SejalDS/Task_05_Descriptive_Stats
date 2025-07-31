# Task_05_Descriptive_Stats

## 📊 Project Overview

This project is part of **Research Task 5: Descriptive Statistics and Large Language Models**, where the objective is to evaluate how accurately a large language model (LLM) such as ChatGPT can answer natural language questions based on a small public dataset. 

For this task, I selected the **2025 Syracuse University Women’s Lacrosse season** data, extracted from publicly available game and player statistics.

The goal is to challenge the LLM with both basic and nuanced questions and validate its responses using Python-based descriptive statistics.

---

## 🧠 Dataset Overview

Four CSV files were used in this project:

- `2025_SU_Lacrosse_Matches_Stats.csv`: Game outcomes, scores, dates, and opponents
- `2025_SU_Lacrosse_Period_Stats.csv`: Team performance per period (goals, shots, saves)
- `2025_SU_Lacrosse_Player_Stats.csv`: Player stats including goals, assists, turnovers, draw controls, etc.
- `2025_SU_Lacrosse_Team_Stats.csv`: Season summary including shot %, clear %, SOG, and more

---

## 🤖 LLM Prompting Strategy

The following types of prompts were tested with the LLM:

| Prompt | Goal |
|--------|------|
| Basic factual | "How many games did SU play?" |
| Decision-making | "Should the coach focus on offense or defense?" |
| Derived metrics | "Who was the most improved player?" |
| Period comparison | "Did SU get worse in later periods?" |
| Efficiency-based ranking | "Who was the most efficient offensive player?" |
| Defensive impact | "Which player had the best transition impact?" |
| Comparative analytics | "In which areas did SU outperform opponents?" |

For each prompt, custom metrics were defined (e.g., `(G+A)-TO`, `(DC+GB)-TO`, etc.) to ensure consistency and interpretability.

---

## ✅ Files Included

- `LLM_Prompts_SU_Lacrosse.md`: All questions, reasoning, and LLM responses with validation
- `scripts/analysis.py`: Python script used to calculate descriptive statistics
- `data/`: Folder containing the four CSV datasets used
- `README.md`: This file

---

## 🔍 Key Findings

- LLMs were able to accurately respond to well-defined, straightforward prompts.
- More complex prompts required metric clarification and validation using Python.
- No neutral site games existed in the dataset, which the LLM correctly interpreted.
- Offensive focus may yield better results, with **Emma Ward** identified as a high-impact player.
- Defensive transition MVP was **Meghan Rode** based on draw controls and ground balls.

---


