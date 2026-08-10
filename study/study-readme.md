# Study Readme

## 1. What It Does

A five-command study toolkit for learning material in plain, simple English, with technical terms explained inline in brackets.

| Command | Purpose |
|---|---|
| /library | Loads reference material, pasted text or an uploaded file, that later commands consult first for the rest of the conversation. |
| /explain | Explains a concept in plain English with at least three distinct examples, kept as in-chat text. |
| /notes | Produces detailed, exam-ready notes delivered as a downloadable Word document. |
| /example | Gives more examples of a topic already being studied, distinct from earlier ones. |
| /quiz | Self-tests on material already covered, one question at a time, with feedback after each answer. |

## 2. How To Invoke

| Method | Example |
|---|---|
| Slash command | Type "/explain", "/notes", "/library", "/example", or "/quiz". |
| Natural phrasing | "Explain this simply", "make notes on this", "quiz me on this", "give me more examples". |
| No topic given | It will ask what topic to cover before doing anything. |

## 3. Sub-Commands

| Command | Effect |
|---|---|
| /library status | Shows what topic and material is currently loaded. |
| /library off | Stops using the loaded material without deleting it. Can be turned back on later. |

## 4. Shared Behaviour Across All Commands

- Difficulty defaults to beginner level unless told otherwise, and the level is remembered for the rest of the conversation.
- /explain defaults to a focused, medium-length answer. /notes defaults to comprehensive.
- If an answer draws from more than one source, such as loaded material, general knowledge, or a web search, it signals which part came from where.
- Before a long output like /notes, it checks the task fits in the remaining conversation and warns if it looks tight.
