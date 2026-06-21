# Prompt Review Checklist

**Use case:** A governance checklist for reviewing any HR prompt before team-wide rollout.
**Owner workflow:** HR AI Governance

## The Checklist

Before any prompt is added to the team library, verify:

- [ ] **No PII in the prompt template.** Variables like [EMPLOYEE_NAME] only where essential.
- [ ] **Anonymity safeguards.** Paraphrase rules for any prompt touching survey or feedback data.
- [ ] **Escalation flags.** The prompt instructs the model to flag, not resolve, sensitive cases.
- [ ] **Legal exposure check.** No outputs that could constitute medical, legal, or
      discriminatory determinations.
- [ ] **Output format specified.** Structure is explicit, reducing inconsistency across users.
- [ ] **Tested by 2 or more team members** on at least 3 realistic inputs each.
- [ ] **Failure mode documented.** The "Notes from real use" section describes when it breaks.

## Why this exists

A prompt library without governance is a liability generator. This checklist was built
alongside an HR team's AI rollout to make adoption safe enough that Legal and the DPO
could sign off on it.
