# Job Application Copilot 🚀
**MSIS 549: AI and GenAI for Business Applications - Assignment 2**

## 📌 Problem Statement
The current status quo for job seekers involves manually cross-referencing their master resume against dozens of job descriptions. Relying on a single, generic LLM prompt (e.g., "Tailor my resume") often leads to hallucinations where the AI invents fake metrics or experiences. 

This **Job Application Copilot** solves this by breaking the task into an agentic workflow of three specialized skills. It diagnoses keyword gaps, surgically rewrites specific bullet points, and generates targeted interview prep—ensuring high Applicant Tracking System (ATS) compatibility while maintaining the strict authenticity of the applicant's real experience.

## 🛠️ System Design (The Skills)
This repository contains a "Skills Pack" (Path A) consisting of three sequential Markdown files:

1. **`jd_analyzer.md` (JD Analyzer & Gap Extractor)** - **Purpose:** Analyzes a target Job Description (JD) against a master resume to identify missing keywords and experience gaps.
   - **Output:** A prioritized "Gap Report."

2. **`resume_tailor.md` (Resume Tailor)** - **Purpose:** Takes the Gap Report and surgically rewrites 2-4 specific resume bullets using the STAR method to naturally incorporate missing keywords.
   - **Constraint:** Strictly prompted to *never* hallucinate metrics or fake experiences.

3. **`interview_prep.md` (Interview Prep Generator)** - **Purpose:** Cross-references the newly tailored resume with the JD's core competencies to generate targeted behavioral interview questions and talking points.

## 🚀 How to Use
These skills are designed to be LLM-agnostic and can be used in Claude, ChatGPT, or any other LLM assistant. 

**Option 1: Standard Chat (ChatGPT / Claude)**
1. Open the raw text of `jd_analyzer.md` and paste it into your chat to initialize the first skill.
2. Provide your Master Resume and the Target Job Description when prompted.
3. Once the Gap Report is generated, paste the text of `resume_tailor.md` into the same chat to initialize the second skill, and provide the specific bullets you want to rewrite.
4. Finally, paste `interview_prep.md` to generate your interview cheat sheet.

**Option 2: Claude Projects / Custom GPTs**
1. Upload these `.md` files as "Project Knowledge" in Claude or as "Instructions" in a Custom OpenAI GPT.
2. Simply
