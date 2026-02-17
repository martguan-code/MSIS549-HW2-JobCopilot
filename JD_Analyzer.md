---
name: jd-analyzer-gap-extractor
description: Analyzes a target Job Description (JD) against a user's master resume to identify missing keywords, underrepresented skills, and experience gaps. Use this as the first step in the tailoring process.
---

# JD Analyzer & Gap Extractor

## Overview
Recruiters and Applicant Tracking Systems (ATS) filter resumes based on specific keyword matches. This skill acts as a diagnostic tool to objectively find what is missing from the master resume before any rewriting begins.

## Inputs
1. `job_description`: The full text of the target job posting.
2. `master_resume`: The user's current, untailored resume text.

## Workflow
1. **JD Extraction**: Scan the `job_description` and extract a prioritized list of Hard Skills (e.g., Python, SQL, Agile) and Soft Skills (e.g., Stakeholder Management, Cross-functional leadership).
2. **Resume Cross-Reference**: Compare the extracted skills against the `master_resume`.
3. **Gap Analysis**: Categorize findings into:
   - *Missing Keywords*: Crucial terms in the JD completely absent from the resume.
   - *Underrepresented Skills*: Skills mentioned briefly but lacking metric-driven impact.
4. **Actionable Output**: Generate a bulleted "Gap Report" detailing exactly which 3-5 keywords must be integrated into the resume.

## Constraints
- Do not rewrite the resume in this step; only output the diagnostic report.
- Strictly rely on the provided text. Do not assume the user has skills not listed in their master resume.

## Example Usage
"Please run the JD Analyzer. Here is the job description for the Microsoft PM role: [JD text], and here is my master resume: [Resume text]."
