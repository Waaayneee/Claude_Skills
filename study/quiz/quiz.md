---
name: quiz
description: Use this skill whenever the user invokes /quiz with study material (pasted text, an uploaded document, or a named topic to cover). Always use this skill for /quiz requests even if phrased slightly differently (e.g. "quiz me on this", "test me on this material") without typing the slash command explicitly. Do not use this skill for /study or /notes requests, those are separate skills.
---

# /quiz

Purpose: test Wayne's understanding of the material.

1. Read through the full material first.
2. Ask how many questions Wayne wants and what format, if not already specified (e.g. multiple choice, short answer, mixed). If unspecified and it is not clear from context, ask before generating.
3. Generate questions that cover the material proportionally, do not cluster all questions around one section.
4. Include a mix of difficulty: recall (definitions, facts), application (worked problems, scenarios), and analysis (why/how, compare/contrast) where the material supports it.
5. Do not reveal answers immediately after each question. Present the full question set first.
6. After the full question set, provide an answer key in a separate section, with a short explanation for each answer, not just the answer alone. For numerical or procedural questions, show the full working in the answer key.
7. Use bordered tables for the answer key if it improves clarity (question number, answer, brief explanation).

## Shared rules

- If no material has been provided yet and `/quiz` is invoked, ask Wayne to paste the material or upload the file before proceeding. Do not generate content from assumption or memory of the topic name alone unless Wayne explicitly says to work from general knowledge on a named topic.
- Never use em dashes, and never write a sentence that would require one.
- Always address Wayne by name first in the response.
- If the material is long enough that completing the full task risks running out of remaining tokens in the conversation, flag this before starting and advise Wayne to open a new conversation if needed.
