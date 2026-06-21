# HR AI Prompt Library

A production-tested collection of prompts for HR workflows, built and refined while
leading AI enablement for the HR team at a global cybersecurity software company.

These aren't theoretical examples. Each prompt was developed for a real recurring HR
task, tested with real stakeholders, and iterated based on the quality of what it
produced.

## What's Inside

| Folder | Contents |
|--------|----------|
| `talent-acquisition/` | Resume analysis, interview question generation, job description drafting |
| `hr-operations/` | Policy summarization, employee communications, case documentation |
| `people-analytics/` | Data interpretation, report narratives, survey analysis |
| `governance/` | AI usage guidelines, prompt review checklists, bias-check prompts |

## Design Principles

Every prompt in this library follows the same structure:

1. **Role and context first.** The model is told who it is and what it knows.
2. **Explicit output format.** Structure is specified, never assumed.
3. **Guardrails inline.** What to avoid is stated in the prompt, not hoped for.
4. **Variables in brackets.** Placeholders like `[JOB_TITLE]` and `[POLICY_NAME]` make
   every prompt reusable.

## Example

From `talent-acquisition/interview-questions.md`:

> You are an experienced technical recruiter preparing structured interview questions.
> Based on the job description below, generate 8 behavioral questions that probe for
> [COMPETENCY_1] and [COMPETENCY_2]. Format as a numbered list with a one-line
> "what a strong answer includes" note under each question. Avoid questions answerable
> with yes/no. Job description: [PASTE_JD]

## Background

I serve as the HR AI subject matter expert at my organization, where I led the team's
transition to Claude and built the internal prompt training program. This library is the
public, sanitized version of that work, with company-specific details removed and the
structure kept intact.

## License

MIT. Use freely, attribution appreciated.
