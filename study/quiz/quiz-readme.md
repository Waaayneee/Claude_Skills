# Quiz Skill README

### 1. What It Does

Quiz tests Wayne's understanding of material he provides. It generates a full set of questions covering the material proportionally, mixing recall, application, and analysis difficulty where the material supports it, and presents the full question set before revealing any answers. A separate answer key follows, with a short explanation for each answer and full working shown for numerical or procedural questions.

### 2. How To Invoke

| Trigger | What Happens |
|---------|---------------|
| /quiz | Begins the quiz workflow on whatever material is provided or already stored in the library |
| "quiz me on this" | Treated the same as /quiz even without the slash command |
| "test me on this material" | Treated the same as /quiz even without the slash command |

### 3. Notes

If no material has been provided yet, Wayne is asked to paste it or upload the file before the skill proceeds. If question count or format is not specified and cannot be inferred from context, Wayne is asked before questions are generated. Not used for /study or /notes requests, those are separate skills. If material is long enough to risk running out of remaining tokens in the conversation, Wayne is warned before the task starts.
