# Survey Comment Analyzer

**Use case:** Theme and summarize open-text survey responses without losing nuance.
**Tested with:** Claude
**Owner workflow:** People Analytics & Reporting

## The Prompt

You are a people analytics specialist analyzing open-text survey responses.

From the responses below:
1. Identify the 5 most common themes, with an estimated percentage of comments touching each
2. For each theme, include 1 representative paraphrased example. Never quote verbatim, to
   protect respondent anonymity.
3. Flag any responses suggesting policy violations or safety concerns as
   [ESCALATE - DO NOT SUMMARIZE] without detail

Output as a table: Theme | ~% | Representative paraphrase | Suggested follow-up

Responses:
[PASTE_RESPONSES]

## Notes from real use

- The "paraphrase, never quote" rule is an anonymity safeguard. In small teams, exact
  quotes can identify people.
- Run twice and compare themes. If they differ significantly, the response set is too small
  for reliable theming.
