---
name: stc
description: Use this skill whenever the user invokes /stc, or asks to turn an STC pre event proposal or event details into an Instagram caption. If invoked and no pre event proposal file or event details have been shared in the conversation, ask the user to upload or paste them before writing anything. Once the source material is available, produce an Instagram caption that follows the fixed STC caption format (hook line, one line pitch, speaker line, what you will gain section, optional workshop requirements section, encouragement and Q&A line, closing hook, and a register in bio closing line).
---

# STC Instagram Caption Writer

Writes an Instagram caption for an STC (Sunway Tech Club, or relevant student tech club) event, workshop, or talk, based on a pre event proposal document and or event details the user provides, following a fixed caption format.

## Workflow

1. Check if a pre event proposal file is attached, or if event details have already been shared in the conversation (event name, speaker, topic, learning outcomes, requirements).
   - If neither is present, ask the user to upload the proposal or paste the event details, and stop. Do not invent an event.
   - If a file is attached, read it in full before writing anything.

2. Extract the following from the source material:
   - Event topic or theme (what the workshop or talk is about)
   - Speaker name, role or title, and company or organisation
   - What attendees will gain or learn (the key takeaways, usually 4 to 6 points)
   - Workshop requirements, if any (things attendees must bring or set up beforehand, e.g. BYOD, software installs, prerequisite knowledge)
   - Any support details (helpers on hand, Q&A session, troubleshooting)

   If any of these are missing from the source material and cannot be reasonably inferred, insert a placeholder in the format [missing info], where "missing info" describes what is needed. Do not fabricate speaker names, companies, or specific figures.

3. Determine whether the workshop requirements section is needed. Only include it if the event genuinely has prerequisites (bring your own device, prior software setup, prior registration steps, etc). If the event has no such requirements (e.g. a talk or panel with no setup needed), skip this section entirely rather than forcing one.

4. Write the caption using this fixed structure, in this order:
   - **Hook line**: one short opening line with a relevant emoji that frames what the event unlocks for the reader (e.g. a backend journey, a design journey, a career first step). Match the emoji to the topic rather than reusing the same one across unrelated events.
   - **One line pitch**: one or two sentences describing what attendees will actually do in the session, ending with one or two relevant emojis.
   - **Speaker line**: on its own line, formatted as: 🎤 Speaker: [Name] ([Role], [Company])
   - **What you'll gain section**: a header line using 🔎 What you'll gain: followed by each takeaway on its own line, each starting with a relevant emoji rather than a bullet character or dash. Match emoji choice to the content of each point.
   - **Workshop Requirements section (only if applicable)**: a header line using ⚠️ Workshop Requirements: followed by each requirement on its own line, each starting with a relevant emoji rather than a bullet character or dash.
   - **Support line**: a short reassurance line mentioning helpers being available and a Q&A session, if the source material confirms these exist. Skip or adjust if not applicable.
   - **Closing hook line**: one short line with 🚀 or another fitting emoji, reinforcing why this is worth attending.
   - **Final call to action line**: a closing line pointing readers to the bio link. Vary the exact wording across different captions rather than always using the same phrase. Acceptable variations include "Register with the link in our bio !!", "Sign up now with the link in our bio", "Save your spot, link in our bio", or similar. Always keep it clearly pointing to the bio link.

5. Writing rules:
   - Never use an em dash anywhere in the caption.
   - Never use a hyphen or dash character (-) anywhere in the caption, including inside bullet style lines. Do not use it to replace an em dash either. Where the source material uses a dash for a list item (e.g. "- BYOD is a MUST"), replace it with a matching emoji instead of a dash.
   - Never write a sentence that would naturally require a dash or em dash. Restructure using a period, comma, or a connecting word instead.
   - Emojis are expected and encouraged throughout this caption format, unlike a normal caption. Use them generously in the hook line, section headers, and each list item, matching the emoji to the meaning of that line.
   - Keep the tone energetic, welcoming, and student facing, matching the tone of the reference caption.
   - Do not pad the caption with generic filler points not supported by the source material.

6. After writing the caption, present it in a plain text block the user can copy directly. Do not wrap it in markdown formatting that would show up when pasted (no bold asterisks, no headers, no code fences shown to the reader beyond the block itself).

7. If the user wants adjustments (different tone, shorter, add or remove a section, swap out the closing line), revise directly without re-asking for the source material.

## Notes

- If multiple events or proposals are attached, ask which one to base the caption on.
- Do not fabricate speaker credentials, company names, attendee numbers, or specific technical claims not present in the source material. Use [missing info] placeholders instead.
- The workshop requirements section is the only optional section in the structure. Every other section (hook line, pitch, speaker line, what you'll gain, support line, closing hook, bio link line) is always included.
- If the user provides a new event for a future caption, treat it as a fresh request and do not carry over details from a previous STC caption in the same conversation.
