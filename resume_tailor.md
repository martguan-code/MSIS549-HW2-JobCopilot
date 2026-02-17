---
name: resume-tailor
description: Rewrites specific resume bullet points to naturally incorporate missing keywords identified by the JD Analyzer, ensuring high ATS compatibility without fabricating experience.
---

# Resume Tailor

## Overview
Taking the diagnostic data from the Gap Extractor, this skill surgically updates specific resume bullet points to align with the target role's vocabulary while maintaining the user's authentic experience.

## Inputs
1. `gap_report`: The output from the JD Analyzer detailing missing/underrepresented keywords.
2. `target_bullets`: 2-4 specific bullet points from the master resume the user wants to upgrade.

## Workflow
1. **Keyword Integration Strategy**: Map the missing keywords from the `gap_report` to the most logically relevant `target_bullets`.
2. **STAR Method Formatting**: Rewrite the selected bullets using the Situation, Task, Action, Result framework. 
3. **Vocabulary Alignment**: Swap generic verbs for the specific action verbs used in the Job Description (e.g., changing "Made" to "Architected" if the JD uses "Architected").
4. **Output Verification**: Present the "Before" and "After" versions of the bullets, explicitly highlighting which new keywords were successfully integrated.

## Constraints
- **Zero Hallucination**: Do NOT invent metrics, job titles, or experiences that were not in the original bullets. 
- Keep rewritten bullets to a maximum of two lines.

## Example Usage
"Using the Gap Report you just generated, please tailor these two bullet points from my previous Data Analyst role to include the keywords 'cross-functional leadership' and 'A/B testing'."
