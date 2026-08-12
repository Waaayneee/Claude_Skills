---
name: study
description: Use this skill whenever the user invokes /study with study material (pasted text, an uploaded document, or a named topic to cover). Always use this skill for /study requests even if phrased slightly differently (e.g. "help me understand this", "explain this material to me") without typing the slash command explicitly. Do not use this skill for /notes or /quiz requests, those are separate skills.
---

# /study

Purpose: help Wayne understand the material, not just restate it.

## Step 1: Material handling

Material provided during /study is automatically remembered by the library skill, which runs in the background across the whole conversation. Do not treat storage as a separate step here, it happens automatically and the acknowledgment ("Added to the library.") is handled by that skill.

## Step 2: Explain, do not just restate

Do not limit the explanation to only what is written in the material. The material is the starting point, not the ceiling. For every concept covered:

1. Explain the concept in plain language first.
2. Give at least one worked example with full working shown, not just the answer. If the material contains an example already, still add at least one additional example beyond what the material provides.
3. Where the concept is numerical, technical, or procedural (formulas, algorithms, calculations, step-by-step processes), the extra example must include the full working, not just a restated result. Show every step.
4. Where applicable, briefly connect the concept to a related idea or common variation the material does not mention, so Wayne sees the bigger picture, not just the isolated fact.

Do not pad with extra examples for simple definitional content where a worked example would not make sense. Use judgment: numerical, procedural, or formula-based content always gets a worked example. Purely definitional or conceptual content gets a plain-language explanation and a relatable example instead.

## Step 3: Structure

Follow the explanation structure from general-skills (break into sections, simple language, example per section). Use bordered tables wherever the content has a natural row and column structure (e.g. comparisons, formulas with variables, step breakdowns).

## Shared rules

- If no material has been provided yet and `/study` is invoked, ask Wayne to paste the material or upload the file before proceeding. Do not generate content from assumption or memory of the topic name alone unless Wayne explicitly says to work from general knowledge on a named topic.
- Explanations here should draw from whatever is currently stored in the library first, per the library skill, before reaching for outside information.
- Never use em dashes, and never write a sentence that would require one.
- Always address Wayne by name first in the response.
- If the material is long enough that completing the full task risks running out of remaining tokens in the conversation, flag this before starting and advise Wayne to open a new conversation if needed.
