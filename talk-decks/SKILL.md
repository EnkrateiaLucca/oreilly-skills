---
name: talk-decks
description: "Prepare talks and presentation decks with the user: audience-first plan, a first draft of the slides with speaker notes, review rounds driven by the user's voice notes, timed practice runs, and a checked export to Google Slides or PowerPoint. Use for a new talk, slide edits on an existing deck, rehearsal planning and reviewing a talk recording."
---

# Talk Decks

Slides the speaker can talk over: one idea per slide, little text, the detail in the speaker notes. Claude drafts fast; the speaker owns the story. This skill gets a good first draft and then follows the speaker's directions. It never replaces their judgment about what the talk is.

> Start from this file, then make it yours: every time you correct the agent, it logs the correction in `FEEDBACK.md`, and corrections you repeat become rules here. See `make-your-own.md` at the root of the repo to build your version from your own past threads.

## Load first

1. The talk's folder, if there is one: the speaker's own notes or brain dump, the event details, past versions. Never overwrite the speaker's notes.
2. Any writing-voice skill the speaker has, for slide text and speaker notes.
3. For a new talk, rehearsal planning or a recording review: [references/preparation-and-rehearsal.md](references/preparation-and-rehearsal.md).
4. `FEEDBACK.md` in this folder: the speaker's past corrections.

## The loop

Initial preparation (once): this skill, built from the speaker's past corrections. Then, for every talk:

1. **Brain dump.** The speaker talks (voice dictation works best) about this audience, the title, the points they must hit, what to avoid, research, numbers, screenshots, real posts this room knows. Start from the room: what should these people leave able to do?
2. **Plan.** A short outline with a one-liner per slide, especially the hook. Iterate on the order before generating any slide. Six lines are cheaper to fix than forty slides.
3. **First draft.** The whole deck end to end, story first, style later. HTML or an artifact is quicker to iterate on than PowerPoint.
4. **Feedback voice notes.** The speaker goes through the deck and dictates one long note per pass, by slide number, with the why. Apply all of it in the same thread.
5. **Practice run.** The speaker says it out loud, timed, end to end. This is where the story breaks: too long, transitions that make no sense, slides with nothing to say. Their next voice note drives the cuts. Repeat 4 and 5 until it holds.
6. **Final pass by hand.** Convert to Google Slides or PowerPoint with real bullet points and build animations, then the speaker fine-tunes while practicing.

## Preparing a new talk

- Write down who is in the room, the format, the real speaking time (and whether Q&A is inside it), and what they should leave able to do. If something is unknown, label it as an assumption instead of inventing it.
- Choose the most relevant real case, not every project the speaker has done. Match examples, humor and jargon to this room.
- Preview the payoff early, then explain the mechanism and its limits.
- Give each section a time budget and mark optional slides. First runs usually go well over: plan with a buffer and cut scope before asking the speaker to talk faster.
- Keep sources, exact numbers and dates in the speaker notes. Separate measured results, personal observations and untested suggestions.

## Editing an existing deck

- A request to add or change content is an edit in place: same slides, same order, same count. Do not merge, move or reorder slides unless the speaker asks.
- If a request could mean content or structure ("combine", "move", "put X in those slides"), ask which one before changing the structure.
- Each new version goes in its own folder or file with a short note of what changed. Never overwrite a version the speaker may present from.

## Style rules

- One title per slide. No small coloured eyebrow line above the title.
- Little text on the slide. What the speaker will say goes in the speaker notes, not in grey sub-text under every box.
- Never show everything on a slide at once. In the final deck, bullets and blocks come in one at a time with build animations.
- Social posts are real screenshots (name and avatar visible), never retyped cards.
- Screenshots say where they come from at a glance. Crop them to what matters.
- Charts have labelled axes. Keep text out of chart images; put labels on the slide.
- Do not highlight one item in a comparison unless asked.
- One strong visual beats a run of near-duplicate slides.
- Examples sit next to the thing they illustrate, not on a separate slide.
- When a slide uses a real example from a past talk, label it (for example "From my last conference talk").
- Labels inside diagrams are slide text, not SVG text: SVG text clips and can't be edited.

## Check before sending

Check every slide in the renderer the audience will actually see, not only your own HTML preview.

- Render each slide to an image and look at it: nothing overflowing, nothing running into the footer, nothing cut at the edges.
- **PowerPoint for Google Slides:** build at 9144000 × 5143500 EMU (16:9) with whole-point font sizes; Google Slides reflows anything else. Render the file (LibreOffice works) and compare side by side with the source.
- Fonts: make sure the fonts used are installed where the deck is rendered, or the layout will shift.

## Output

- The deck (artifact link, .pptx or PDF) plus a short outline of what changed and where.
- For planning or rehearsal requests: the outline, speaking cues or timed review asked for, not an unrequested deck.
- For a recording review: say what was actually watched (transcript span, timestamps, audio or video), attach timestamps to findings, and separate observations from recommendations.

## Guardrails

- Never invent numbers, quotes or dates. Date every number that can change (as of YYYY-MM-DD) and keep its source in the notes.
- Never change a deck's structure without a yes.
- Never send a deck that has not been checked slide by slide in its real renderer.

## Feedback log

After each run, add an entry to `FEEDBACK.md`: date, what was asked, what the speaker corrected (their words), and the status. When the same correction shows up twice, or the speaker states it as a rule, move it into this file and mark the entry as promoted.
