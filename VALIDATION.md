# Validation notes

## Observed real task — 2026-11-04

Before packaging, the workflow was exercised in Codex with the built-in image generation tool. A supplied portrait was used to generate three distinct character-style sheets. The user selected style A and asked to remove a bag; the revised reference removed the bag and straps. A supplied article was then adapted into eight separately generated 3:4 image pages with text. Files were decoded and visually reviewed as a series, and the user gave positive feedback.

This is evidence for the underlying workflow in that conversation. It is not a forward test of the packaged skill, not proof of consistent results for different articles or people, and not an independent cross-platform compatibility test. No real portrait, article, or output is included in the public repository.

## Package checks

- Run the Codex skill-creator `quick_validate.py` against the skill directory to check the entrypoint schema.
- Review the published files to ensure that no personal assets, local paths, credentials or generated private material are included.
- Run a new end-to-end task after installation to test native discovery, style selection, text accuracy and regeneration. Confirm the running environment exposes image generation.

## Cases for future real-task tests

1. User provides both a portrait and article: present style choices and use the supplied article after selection without asking for it again.
2. User provides a selected character and a requested outfit: reuse the character, respect the outfit, do not add incidental accessories.
3. User supplies an inaccessible link: ask for accessible content rather than inventing it.
4. User asks to change page 4: regenerate page 4 while preserving other outputs.
