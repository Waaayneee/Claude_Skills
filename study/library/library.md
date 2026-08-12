---
name: library
description: Always-active background behavior. Trigger automatically whenever Wayne adds new study material to the conversation, whether pasted, uploaded, or provided during /study, /notes, /quiz, or plain chat. Also trigger on every question Wayne asks afterward, in any command or plain chat, to check stored material before searching elsewhere. This skill has no direct command, it runs silently in the background for the rest of the conversation once material has been added.
---

# Library

Background behavior that keeps track of study material Wayne adds to a conversation and prioritizes it as the first source of truth for anything he asks afterward.

## Behavior 1: Remember new material

Whenever Wayne adds new material to the conversation (pasted text, an uploaded file, or content generated earlier in the same chat), treat it as stored for the rest of the conversation. No separate action is needed to save it, it is simply held in context and treated as reference material going forward.

Acknowledge this in one very short, concise sentence, nothing more. Do not describe what the library is or how it works.

Example acknowledgment:
```
Added to the library.
```

If material is added mid conversation while other material is already stored, both remain available. Do not discard earlier material unless Wayne says to remove or replace it.

## Behavior 2: Check the library first

For any question Wayne asks after material has been added, whether inside /study, /notes, /quiz, or plain chat:

1. Check the stored material first. If the answer is there, answer from it directly.
2. Only search elsewhere (web search, general knowledge) if the stored material does not cover the question, or Wayne explicitly asks for outside information.
3. If the answer partly comes from stored material and partly needs outside information, say which part came from the material and which part did not, briefly, without making it a long disclaimer.
4. If nothing has been added to the library yet, skip this behavior entirely and answer normally.

## Notes

- This skill has no slash command. It is not invoked directly, it activates automatically the moment material is added and stays active for the rest of the conversation.
- This applies across the whole conversation, not just within a specific command.
- Never use em dashes, and never write a sentence that would require one.
- Always address Wayne by name first in the response.
