---
name: notes
description: Use this skill whenever the user invokes /notes with study material (pasted text, an uploaded document, or a named topic to cover). Always use this skill for /notes requests even if phrased slightly differently (e.g. "make notes from this", "summarize this into notes") without typing the slash command explicitly. Do not use this skill for /study or /quiz requests, those are separate skills.
---

# /notes

Purpose: produce condensed, structured study notes from the material.

1. Read through the full material first before writing anything.
2. Organize notes under clear numbered or lettered headings that mirror the structure of the material (do not reorganize the material's own structure unless it is genuinely disordered).
3. Keep notes concise. Notes summarize and compress, they do not re-explain at length.
4. Use bordered tables for any content with a natural row and column structure (definitions, comparisons, formulas, steps).
5. Bold key terms on first mention.
6. Do not add outside examples or extra explanation beyond the material unless a term is used without being defined in the material, in which case add a short one-line definition only.
7. End with a short "Key Takeaways" section, no more than 5 to 7 bullet points, summarizing the most exam-relevant points.

## Shared rules

- If no material has been provided yet and `/notes` is invoked, ask Wayne to paste the material or upload the file before proceeding. Do not generate content from assumption or memory of the topic name alone unless Wayne explicitly says to work from general knowledge on a named topic.
- Never use em dashes, and never write a sentence that would require one.
- Always address Wayne by name first in the response.
- If the material is long enough that completing the full task risks running out of remaining tokens in the conversation, flag this before starting and advise Wayne to open a new conversation if needed.
