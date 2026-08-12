# STC Instagram Caption Skill

## What this does

Invoke with /stc. Reads an STC pre event proposal document and or event details pasted in chat, then produces an Instagram caption for the event following a fixed format.

## Trigger

- /stc
- Any request to turn an STC pre event proposal or event details into an Instagram caption

## Input needed

- A pre event proposal file, and or
- Event details typed or pasted directly in chat (event topic, speaker name and role, what attendees will gain, any requirements)

If neither is available when /stc is invoked, the skill will ask for it before writing anything.

## Output format

1. Hook line with emoji
2. One line pitch with emoji
3. Speaker line (🎤 Speaker: Name, Role, Company)
4. What you'll gain section (🔎), each point on its own line with a matching emoji
5. Workshop Requirements section (⚠️), only included if the event actually has requirements
6. Support line (helpers and Q&A, if applicable)
7. Closing hook line (🚀)
8. Final call to action line pointing to the bio link, wording varies each time

## Hard rules

- No em dash, ever
- No hyphen or dash character (-) anywhere, including in place of list bullets
- No sentence restructured to need a dash either
- Emojis are used generously in this skill, this is an exception to the general no emoji preference since the reference format is emoji heavy
- Workshop Requirements is the only optional section, everything else is always included
- No fabricated speaker names, companies, or figures, use [missing info] placeholders instead

## Revisions

Once a caption is written, ask for adjustments directly (tone, length, drop or add a section, different closing line) without needing to re-upload the source material.
