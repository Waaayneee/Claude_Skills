# Export Chat Readme

## 1. What It Does

Compiles the current conversation into a single downloadable Markdown file, so another person can upload it into a new Claude chat and continue the work as a handoff.

OR more unethically, it kinda allows you to abuse free Claude accounts

## 2. How To Invoke

| Trigger Phrase | Result |
|---|---|
| "/export-chat" | Exports handoff file. |
| "export claude" | Generates and delivers the handoff file. |
| "export chat" / "export this chat" | Same result, alternate phrasing. |
| Asking how to export | Reminds you the trigger phrase is "export claude". |

## 2.2 How To Use
1. **BEFORE** you hit the usage limit around 90% usage left (better if lesser to be safe) use "/export-chat"
2. Download the markdown file (.mdf).
3. Switch to another account with more tokens.
4. Drop the markdown file (.mdf) into. the chat
5. Continue the conversation (may need to add additional context).


## 3. File Contents

The exported file includes a summary of the conversation, key context and constraints, work completed so far, open questions, where things left off, and a full raw transcript.

## 4. Notes

The export does not restore live memory, artifacts, or tool call history. Only what is written in the file carries over to the new chat. If the conversation is very long, the summary sections are prioritised over the full transcript, and this trade-off is flagged before the file is generated.
