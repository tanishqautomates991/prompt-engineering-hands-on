# Prompt Engineering Hands-On Assessment

**Author:** Tanishq Soni  
**Project Title:** Prompt Engineering Hands-On Course – Assessment

---

## Project Overview
This repository contains the assets for the **Prompt Engineering Hands-On Course** assessment. The goal was to demonstrate how systematic prompt engineering improves the quality of six distinct marketing content types.

| Content Type          | Prompt Technique Used                                          |
|-----------------------|---------------------------------------------------------------|
| Blog Post             | RGCCO Framework + Style Transfer                               |
| LinkedIn Post         | Role Prompting + Zero-Shot with Strict Constraints             |
| Email Campaign        | Few-Shot Prompting                                            |
| Instagram Caption     | Few-Shot Prompting with Negative Constraints                    |
| YouTube Script        | Role Prompting + RGCCO                                         |
| Product Description   | Feature-to-Benefit Mapping + Constraints                       |

The repository includes:
- `prompt_library.md` – the full library of **Before** (naïve) and **After** (engineered) prompt templates.
- `generated_content.md` – the final outputs generated with the optimized prompts.
- `improvement_report.md` – a quantitative comparison (scores / 20) plus a qualitative analysis of each task.
- `README.md` – this overview and usage guide.

---

## Loom Video Walkthrough
A short Loom video walks through the assessment workflow:

- Introduction and list of content types
- Review of a complex prompt (RGCCO blog post)
- Live execution of an optimized prompt
- Presentation of the before‑vs‑after score table

**Loom Video Walkthrough URL:** [https://www.loom.com/share/8f2262fb0d34457ab8a4798bc88358ea](https://www.loom.com/share/8f2262fb0d34457ab8a4798bc88358ea)

---

## How to Use the Prompt Templates
1. Clone or download this repository to your local machine.
2. Open `prompt_library.md` in your preferred editor (VS Code, Sublime, etc.).
3. Locate the **“After (Optimized)”** section for the content type you want to generate.
4. Replace bracketed variables (`[Topic]`, `[Reference Text]`, `[Persona]`, etc.) with your own values.
5. Copy the full prompt (including Role, Goal, Context, Constraints, and Output Format).
6. Paste the prompt into a ChatGPT session (or any compatible LLM) and send it.
7. The model will return content that follows the exact structure and constraints you defined.

> **Tip:** Keep the constraints strict (e.g., word limits, no emojis) to ensure consistent, production‑ready output.

---

## Repository Structure
```
prompt-engineering-portfolio/
├─ prompt_library.md
├─ generated_content.md
├─ improvement_report.md
├─ before_prompts.txt
├─ after_prompts.txt
└─ README.md
```

---

## Getting Started
```bash
# Clone the repository
git clone https://github.com/tanishqautomates991/prompt-engineering-portfolio.git
cd prompt-engineering-portfolio

# Open the prompt library
code prompt_library.md    # or any editor of your choice
```
Then follow the **How to Use the Prompt Templates** steps above.
