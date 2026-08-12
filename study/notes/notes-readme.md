# Notes Skill README

### 1. What It Does

Notes produces condensed, structured study notes from material Wayne provides. It mirrors the material's own structure under numbered or lettered headings, bolds key terms on first mention, and uses bordered tables for anything with a natural row and column structure. It ends with a short Key Takeaways section of up to 5 to 7 points. Unlike /study, which expands on material, /notes compresses it.

### 2. How To Invoke

| Trigger | What Happens |
|---------|---------------|
| /notes | Begins the notes workflow on whatever material is provided or already stored in the library |
| "make notes from this" | Treated the same as /notes even without the slash command |
| "summarize this into notes" | Treated the same as /notes even without the slash command |

### 3. Notes

If no material has been provided yet, Wayne is asked to paste it or upload the file before the skill proceeds. No outside examples or extra explanation are added beyond the material, except a short one-line definition if a term is used without being defined. Not used for /study or /quiz requests, those are separate skills. If material is long enough to risk running out of remaining tokens in the conversation, Wayne is warned before the task starts.
