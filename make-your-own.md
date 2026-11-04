# Make your own talk-decks skill

The skill in this repo is a starting point. The version that works is the one made of **your** corrections. If you have built decks with Claude Code, Codex or another agent before, your past threads already hold them: every "no, keep the slides as they were" and every "this slide has too much text".

Paste this prompt into Claude Code (or Codex) on the machine where those threads live. It reads your history, so check what it quotes before you share the result.

```text
I want a skill for building my talks and slide decks, made from my own past corrections.

1. Find my past threads where we worked on a presentation, a deck, slides or a talk.
   For Claude Code they are the .jsonl files under ~/.claude/projects/; for Codex,
   under ~/.codex/sessions/. List the threads you found (date, talk, number of my
   messages) before going further.
2. In those threads, find every message where I asked for a change, corrected you,
   or repeated a request. Quote my exact words with the date and the talk.
3. Group them into rules: how I plan a talk, how I want slides to look, how I want
   edits made, what you must check before sending me anything. Only keep rules that
   my own messages support, and keep one or two quotes as evidence for each.
4. Write a skill folder:
   - talk-decks/SKILL.md: frontmatter (name, description), when to use it, my loop
     from brain dump to final deck, the rules, and the checks before sending.
   - talk-decks/FEEDBACK.md: one dated entry per correction you found
     (asked, corrected in my words, lesson, status).
   Start from https://github.com/louisfb01/talk-decks-skill if it helps, but my
   rules win wherever they differ.
5. Show me the rules with their quotes so I can confirm each one before you save.

From now on, after each deck we work on, add what I corrected to FEEDBACK.md.
When the same correction shows up twice, move it into SKILL.md.
```

Tips:

- Do it once you have a few decks behind you. Three or four threads of real feedback beat any template.
- Talk your feedback out loud while building the next deck (Wispr Flow, Superwhisper, or your OS dictation). Long voice notes by slide number give the skill much better material than short typed fixes.
- Keep private things out: the prompt quotes your messages, so read the result before you push it anywhere public.
