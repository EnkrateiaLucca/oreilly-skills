# Week 3: HTML artifacts

O'Reilly Skills Live, Nov 24, 2026. Lucas Soares on HTML artifacts: single-file pages your agent builds so you can see its work, steer it, and hand your decisions back.

## Slides

- [html-artifacts-deck.pdf](html-artifacts-deck.pdf): one page per scene, readable on GitHub.
- [slides/html-artifacts-deck.html](slides/html-artifacts-deck.html): the animated deck itself, which is also an HTML artifact. Download the `slides/` folder, open the file in a browser and press → to step through it.

## Live examples from the class

Claude artifacts you can open in the browser:

| Example | What it shows |
| --- | --- |
| [The Plan in Motion](https://claude.ai/artifact/UfR2P2SrJVsM2KbYqmb6vH) | A city mobility plan (PMUS Las Rozas 2022–2030) turned into a 3D model you walk through chapter by chapter |
| [Rhythm Lanes](https://claude.ai/artifact/1Q7gftpvjJYqYrBVBMXWwy) | A piano rhythm trainer with a metronome. Press Start and try 3 against 2 |
| [Mirage rulebook](https://claude.ai/artifact/RsrDRPrS7B2a21cjRbeiQJ) | Rules for an AI party game, with a playable round at the top |
| [Muffin tray morph](https://claude.ai/artifact/359121i26u6Gkix7XQNcYD) | An 11-second explainer animation: muffins into cookies |

The other examples in the deck (morning brief, review pages, lessons, the email plan) run on personal data, so they appear only as screenshots.

## Sources mentioned

- Simon Willison, [Useful patterns for building HTML tools](https://simonwillison.net/2025/Dec/10/html-tools/)
- Thariq Shihipar, [The unreasonable effectiveness of HTML](https://thariqs.github.io/html-effectiveness/), with the two demos from the deck: [three approaches side by side](https://thariqs.github.io/html-effectiveness/01-exploration-code-approaches.html) and [a prompt tuner](https://thariqs.github.io/html-effectiveness/20-editor-prompt-tuner.html)
- Konstantin Saifo, [a floor plan turned into a live 3D warehouse twin](https://x.com/konstantinsaifo/status/2112103898693427587)

## Try it

Add these three sentences to your next prompt:

> Make it one HTML file. No React, no build step.
> Show me 3 options side by side so I can point at one.
> End with a Copy button that hands my choices back to you.

Five rules for a good artifact: one file, one job, options side by side, inputs over prose, end with export. When you build the same interaction twice, turn it into a skill.
