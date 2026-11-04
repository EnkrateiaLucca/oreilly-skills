# Feedback log

Your agent adds an entry after each run of the skill. When the same correction appears twice, or you state it as a rule, it moves into `SKILL.md` and the entry is marked `promoted`.

Format:

```
### YYYY-MM-DD: short title
- Asked: what you asked for, in a line.
- Corrected: what you changed or said, in your own words.
- Lesson: the rule this suggests.
- Status: logged | promoted YYYY-MM-DD
```

Examples from the author's own log (shortened, quotes verbatim):

### 2026-10-01: content request read as a structure change
- Asked: "put proof I know my stuff in those slides".
- Corrected: "no no i didnt want to change placement it was good as it was". Two slides had been merged and moved.
- Lesson: adding content is an edit in place; ask before changing the structure.
- Status: promoted

### 2026-10-08: the .pptx broke in Google Slides
- Asked: export the deck as .pptx for Google Slides.
- Corrected: "you need to check the slides before sending me, they are horrible". Text wrapping and overlays broke in Google Slides.
- Lesson: build at 9144000 × 5143500 EMU with whole-point font sizes and check in a real renderer.
- Status: promoted

### 2026-11-04: everything on the slide at once
- Asked: review of the Google Slides step of a deck.
- Corrected: "I never want everything on a slide to show at once."
- Lesson: bullets and blocks come in with build animations.
- Status: promoted
