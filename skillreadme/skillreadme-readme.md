# Skillreadme README

## 1. What It Does

Generates a README for an existing skill by reading that skill's SKILL.md file directly, no need to describe the skill manually. The output always follows the same fixed three-section format: what it does, how to invoke, and notes, then saves the file right away with no chat preview or confirmation step.

## 2. How To Invoke

| Trigger | What Happens |
|---|---|
| /skillreadme | Documents whichever skill was most recently built or edited earlier in this conversation |
| /skillreadme <skillname> (e.g. /skillreadme linkedin) | Documents that named skill instead of defaulting to the most recent one |
| /skillreadme with no named skill and nothing built or edited yet in the conversation | Asks which skill to document before doing anything else |

## 3. Notes

- Pulls triggers, commands, and caveats straight from the target skill's SKILL.md, nothing is invented if it isn't in the file.
- Generates and saves the README directly, it does not wait for review before writing the file.
- Output file follows the naming convention `<skillname>-readme.md` and is saved in the same folder as that skill's SKILL.md.
- If the named or defaulted skill can't be found, it asks you to confirm the skill name instead of guessing.
