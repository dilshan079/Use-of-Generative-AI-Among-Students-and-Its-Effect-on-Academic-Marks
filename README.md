# Use-of-Generative-AI-Among-Students-and-Its-Effect-on-Academic-Marks
# Generative AI Use & Student Outcomes Analytics

An end-to-end interactive dashboard and analytical dataset study examining how Generative AI tool usage impacts academic performance, skill retention, burnout risk, and mental health across 50,000 higher education students.

---

## Executive Summary

This study analyzes 50,000 student records across 5 academic majors and 5 study levels to understand the relationship between AI adoption habits and educational outcomes.

### Key Metrics Overview
* **Total Cohort Analyzed:** 50,000 Students
* **Average Weekly GenAI Usage:** 8.4 Hours/Week (Median: 5.8 hrs, Max: 40 hrs)
* **Average Traditional Study:** 11.2 Hours/Week
* **Average GPA Improvement:** +0.20 points (3.15 → 3.35)
* **Average Skill Retention Score:** 75.8 / 100
* **Paid Subscription Adoption:** 42.3%
* **Burnout Risk Distribution:** Low: 32.7% | Medium: 42.3% | High: 25.0%

---

## Core Findings & Insights

1. **Moderate Use Wins (Sweet Spot):**
   * GPA gains peak at **5–15 hours/week (+0.23 GPA gain)**.
   * Usage exceeding 20 hours/week diminishes returns (+0.16 GPA gain).

2. **Heavy Use Erodes Skills & Elevates Burnout:**
   * Skill retention drops from **77.1** (5–10 hrs) down to **70.3** (20+ hrs).
   * **74% to 90%** of heavy users (30–40 hrs) show **High Burnout Risk**, compared to just **9%** for light users (0–2 hrs).

3. **Prompt Engineering Skill Impact:**
   * Advanced prompt engineers retain significantly more skills (**82.1** vs **71.1** for beginners) and achieve higher GPA gains (**+0.25** vs **+0.19**).

4. **Use-Case Breakdown Matters:**
   * **Debugging / Troubleshooting:** Highest GPA gain (+0.25) & retention (78.1).
   * **Direct Answer Generation:** Lowest GPA gain (+0.13) & retention (73.7).

5. **Institutional Policy Paradox:**
   * Strict AI bans do not stop usage, but increase **exam anxiety (4.9 vs 4.1)** and slightly reduce GPA gains (**+0.19 vs +0.21**).

---

## Key Data & Visualizations

### 1. Usage Intensity vs Outcomes
| Weekly GenAI Hours | Students Count | Avg GPA Change | Skill Retention | Exam Anxiety (1-10) |
| :--- | :--- | :--- | :--- | :--- |
| **0–2 hrs** | 10,740 | +0.19 | 75.6 | 3.8 |
| **2–5 hrs** | 11,852 | +0.20 | 76.3 | 3.9 |
| **5–10 hrs** | 12,173 | +0.23 | 77.1 | 4.1 |
| **10–20 hrs** | 10,229 | +0.22 | 76.6 | 4.8 |
| **20+ hrs** | 5,006 | +0.16 | 70.3 | 5.6 |

---

### 2. Major Segment Breakdown
| Major | Students | Avg AI Hours/Wk | GPA Change | Retention Score | Anxiety | AI Dependency | % High Burnout |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **STEM** | 15,059 | 10.5 | +0.217 | 76.8 | 4.43 | 3.79 | 30.0% |
| **Business** | 12,538 | 8.3 | +0.194 | 75.3 | 4.25 | 3.49 | 24.3% |
| **Humanities** | 9,994 | 6.8 | +0.198 | 75.3 | 4.14 | 3.24 | 20.7% |
| **Medical** | 6,476 | 7.5 | +0.201 | 75.5 | 4.23 | 3.40 | 23.2% |
| **Arts** | 5,933 | 7.3 | +0.197 | 75.7 | 4.17 | 3.36 | 22.7% |

---

### 3. Primary Use Case Impact
| Primary Use Case | Share (%) | GPA Change | Skill Retention |
| :--- | :--- | :--- | :--- |
| **Debugging / Troubleshooting** | 24.6% | +0.25 | 78.1 |
| **Copywriting / Drafting** | 24.0% | +0.20 | 75.2 |
| **Ideation** | 21.4% | +0.20 | 75.5 |
| **Summarizing Reading** | 17.3% | +0.20 | 75.2 |
| **Direct Answer Generation** | 12.7% | +0.13 | 73.7 |

---

## Dataset Schema (`data/ai.csv`)

The dataset includes 50,000 anonymized student records with the following fields:

* `student_id`: Unique identifier for each student record.
* `major`: Academic field (`STEM`, `Business`, `Humanities`, `Medical`, `Arts`).
* `year_of_study`: Academic year (`Freshman`, `Sophomore`, `Junior`, `Senior`, `Graduate`).
* `weekly_genai_hours`: Number of hours spent using Generative AI per week.
* `traditional_study_hours`: Number of hours spent in traditional studying per week.
* `primary_use_case`: Main purpose of AI usage (e.g., `Debugging`, `Copywriting`, `Direct Answer Generation`).
* `prompt_skill_level`: Proficiency in AI prompting (`Beginner`, `Intermediate`, `Advanced`).
* `num_ai_tools`: Number of distinct AI tools utilized (1 to 5+).
* `institutional_policy`: Policy enforced (`Strict Ban`, `Allowed with Citation`, `Actively Encouraged`).
* `gpa_pre`: Student GPA before the semester.
* `gpa_post`: Student GPA after the semester.
* `gpa_change`: Differential GPA gain ($gpa\_post - gpa\_pre$).
* `skill_retention`: Measured score out of 100.
* `exam_anxiety`: Perceived exam anxiety score (Scale 1–10).
* `ai_dependency`: Perceived dependency score.
* `burnout_risk`: Categorical risk classification (`Low`, `Medium`, `High`).

---
