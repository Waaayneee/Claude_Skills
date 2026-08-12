---
name: skillreadme
description: Use this skill whenever the user invokes /skillreadme. Generates a README file for a skill, following a fixed three-section format (what it does, how to invoke, notes). If the user names a skill in the command (e.g. "/skillreadme linkedin"), document that skill. If no skill is named, default to whichever skill was most recently built or edited earlier in this conversation. If neither is available (no skill named and none built or edited yet in this conversation), ask the user which skill to document before proceeding.
---

# Skill README Generator

Generates a README for an existing skill by reading its SKILL.md file directly, following a fixed three-section format: what it does, how to invoke, and notes.

## Workflow

1. Determine the target skill:
   - If the user names a skill in the command (e.g. "/skillreadme linkedin"), use that skill.
   - If no skill is named, default to whichever skill was most recently created or edited earlier in this conversation.
   - If neither applies (no skill named and no skill built or edited yet in this conversation), ask the user which skill to document, then stop and wait for their answer.

2. Locate and read that skill's SKILL.md file directly (check the conversation's working files first if the skill was just created and not yet saved to /mnt/skills/user/, otherwise read it from /mnt/skills/user/<skillname>/SKILL.md). Do not ask the user to describe the skill, pull everything from the file itself.

3. Generate the README using exactly these three sections, in this order:

   ### 1. What It Does
   A short, plain-language explanation of the skill's purpose and what it produces. Two to four sentences, no filler.

   ### 2. How To Invoke
   A fully bordered table (every cell wall filled in, no open borders) with two columns:
   - **Trigger**: the exact command (e.g. /linkedin) plus any keyword phrases or natural-language variants that also trigger the skill.
   - **What Happens**: a short description of what that trigger does.
   Pull the trigger commands and keywords straight from the skill's frontmatter description and workflow steps, do not invent triggers that are not in the file.

   ### 3. Notes
   Any caveats, requirements, or dependencies mentioned in the SKILL.md (e.g. "requires a photo to be attached", "only works with skills already in /mnt/skills/user/"). If the skill has no notable caveats, keep this section brief rather than padding it.

4. Formatting rules:
   - No em dashes anywhere, and no sentences restructured around double hyphens either.
   - No emojis.
   - Fully bordered tables only, every cell wall filled in.
   - Use the naming convention `<skillname>-readme.md` for the output file (e.g. linkedin-readme.md).

5. Create the file directly at `<skillname>-readme.md` (same folder as the skill's SKILL.md), no chat preview or confirmation step needed, then present it to the user.

## Notes

- Never fabricate triggers, commands, or notes that are not actually present in the target SKILL.md, if something is unclear or missing, leave it out rather than guessing.
- If the named or defaulted skill cannot be found anywhere in the conversation or in /mnt/skills/user/, tell the user and ask them to confirm the skill name instead of guessing.
- This skill generates and saves the README directly, it does not wait for review before writing the file.
