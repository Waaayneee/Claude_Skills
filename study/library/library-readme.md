# Library Skill README

### 1. What It Does

Library is an always-active background skill that remembers study material Wayne adds to a conversation, whether pasted, uploaded, or provided during /study, /notes, /quiz, or plain chat. Once material is added, it acknowledges storage in one short sentence and then prioritizes that stored material as the first source checked for any question Wayne asks afterward, only reaching for outside information if the material does not cover it.

### 2. How To Invoke

| Trigger | What Happens |
|---------|---------------|
| Adding new material anywhere in the conversation (pasted text, uploaded file, or content generated earlier in the chat) | Material is automatically remembered for the rest of the conversation, acknowledged with a short line such as "Added to the library." |
| Any question asked after material has been added, inside /study, /notes, /quiz, or plain chat | The stored material is checked first. If it covers the question, the answer comes from it directly. Outside information is only used if the material does not cover it or Wayne explicitly asks for outside information |

### 3. Notes

This skill has no slash command and cannot be invoked directly, it runs automatically the moment material is added and stays active for the rest of the conversation. If nothing has been added to the library yet, this behavior is skipped and Claude answers normally. If an answer is partly from stored material and partly from outside information, the split is noted briefly.
