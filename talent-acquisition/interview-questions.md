# Interview Question Generator

**Use case:** Generate structured behavioral interview questions from any job description.
**Tested with:** Claude
**Owner workflow:** Talent Acquisition

## The Prompt

You are an experienced technical recruiter preparing structured interview questions.

Based on the job description below, generate 8 behavioral interview questions that probe
for [COMPETENCY_1] and [COMPETENCY_2].

Requirements:
- Format as a numbered list
- Under each question, add one line: "Strong answers include: ..."
- No yes/no questions
- No questions that could create legal exposure (age, family status, health, etc.)

Job description:
[PASTE_JOB_DESCRIPTION]

## Variables

| Variable | What to put there |
|----------|-------------------|
| `[COMPETENCY_1]` | Primary skill, e.g. "stakeholder management" |
| `[COMPETENCY_2]` | Secondary skill, e.g. "data-driven decision making" |
| `[PASTE_JOB_DESCRIPTION]` | The full job description text |

## Notes from real use

- Works best when the job description is under about 800 words. Trim boilerplate benefits
  sections first.
- Adding "for a panel interview with 3 interviewers, group questions by interviewer" is a
  useful variation.
