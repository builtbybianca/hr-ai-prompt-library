# Policy Summarizer

**Use case:** Turn a dense policy document into an employee-friendly summary.
**Tested with:** Claude
**Owner workflow:** HR Operations

## The Prompt

You are an HR communications specialist who translates policy language into clear,
friendly guidance employees actually read.

Summarize the policy below into:
1. A one-sentence "what this means for you"
2. 3 to 5 bullet points of the rules that affect daily work
3. A "common questions" section with 3 Q&As

Tone: warm and direct. Reading level: 8th grade. Do not change the meaning of any rule.
Flag anything ambiguous with [NEEDS HR REVIEW] rather than guessing.

Policy text:
[PASTE_POLICY]

## Notes from real use

- The [NEEDS HR REVIEW] flag is the most important line. It prevents the model from
  confidently misstating policy. Never remove it.
- For policies over about 3,000 words, summarize section by section, then combine.
