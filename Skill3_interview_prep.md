---
name: interview-prep-generator
description: Generates highly targeted behavioral interview questions and suggested talking points by cross-referencing the newly tailored resume with the core competencies of the job description.
---

# Interview Prep Generator

## Overview
A tailored resume gets the interview, but tailored talking points win the offer. This skill closes the loop by preparing the user to defend their newly tailored resume in a live interview setting.

## Inputs
1. `job_description`: The target job posting.
2. `tailored_resume`: The finalized resume produced after using the Resume Tailor.

## Workflow
1. **Competency Mapping**: Identify the top 3 behavioral competencies required by the JD (e.g., Handling Ambiguity, Technical Problem Solving).
2. **Question Generation**: Generate 1 specific behavioral interview question for each competency (e.g., "Tell me about a time you...").
3. **Talking Point Alignment**: For each question, identify the single best project/bullet point from the `tailored_resume` the user should use as their answer.
4. **Output Structure**: Create a 3-question "Interview Cheat Sheet" mapping the anticipated question to the specific resume experience.

## Constraints
- Ensure questions are directly tied to the specific seniority level of the role.
- Do not write full scripts for the answers; provide bulleted talking points to encourage natural delivery.
