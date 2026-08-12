# Study Skill README

### 1. What It Does

Study helps Wayne understand material rather than just restate it. Material provided is automatically remembered by the library skill in the background. For every concept in the material, it gives a plain-language explanation, and for numerical, technical, or procedural concepts it adds at least one extra worked example with full working shown, beyond whatever example the material already has. Where relevant, it also briefly connects a concept to a related idea the material does not cover.

### 2. How To Invoke

| Trigger | What Happens |
|---------|---------------|
| /study | Begins the study workflow on whatever material is provided or already stored in the library |
| "help me understand this" | Treated the same as /study even without the slash command |
| "explain this material to me" | Treated the same as /study even without the slash command |

### 3. Notes

If no material has been provided yet, Wayne is asked to paste it or upload the file before the skill proceeds, it does not generate content from memory of a topic name alone unless Wayne explicitly asks to work from general knowledge. Explanations draw from the library skill's stored material first before reaching for outside information. Not used for /notes or /quiz requests, those are separate skills. If material is long enough to risk running out of remaining tokens in the conversation, Wayne is warned before the task starts.
