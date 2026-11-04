---
name: ip-picture-workshop
description: Turn a supplied portrait and article, notes, script, story, or other text into a multi-page illustrated social carousel featuring a consistent personal IP character. Use when a user wants a photo-based character style and image cards for Xiaohongshu, WeChat, or similar channels, or asks to turn text into IP comics. Requires an available image-generation tool.
---

# IP 图文工坊

Create a reusable illustrated character from the user's photo, then turn their text into complete illustrated image cards with the words generated in the image. Default to the user's language. A different topic, page count, format, or visual style is welcome.

## Choose a character

- If the user supplies an existing selected character reference, use it. Otherwise ask for a photo or a local image path. If they cannot provide one, accept their character description.
- Use the photo primarily for identity: recognizable face, hair and expression. Do not carry over incidental bags, straps or other accessories unless requested. Follow explicitly requested clothing; otherwise the photo's clothes or an outfit appropriate to the chosen style are both acceptable. Do not infer identity, age, occupation or personality from appearance.
- Use the available built-in image generation capability and read its current instructions if available. Make **three separate style sheets** by default, each with multiple expressive poses of the same recognizable person. Choose distinct useful aesthetics, such as clean line-art, warm hand-drawn and expressive chibi, unless the user gives different directions. Keep character references without incidental bags. Generate each sheet using the user-supplied photo as a reference.
- Show the actual images with short labels. Let the user pick or request changes. Do not select for them. A provided or previously approved selection is sufficient; do not ask again. Retain the selected reference and its style in the task's files so it can be reused. Never assume another chat can access an unsaved profile or source.

## Turn text into pictures

1. Once the character is selected, ask for the article, text, document or link if not already supplied. Read actual content; for inaccessible links, explain and ask for pasted text or a file. Do not invent the contents or claim an inaccessible link was read.
2. Analyze the argument, narrative and emotional tone. Plan a concise sequence internally: cover, key points, examples or contrasts, and a satisfying ending as appropriate. Choose page count by content, platform and user instructions; 6–9 is a starting point for a substantial article, not a hard limit. Keep the source's meaning and distinguish direct quotations from paraphrase. Do not add unsupported claims, statistics, sources or endorsements. Avoid sensational headlines that misrepresent the text.
3. Unless the user asks to review an outline, proceed directly to generation. Use the selected character image as a reference for each page; include the photo as an identity reference if useful and available. Keep face, distinctive hair and visual language consistent without treating clothing as immutable if the user asks to change it. Respect all requested content, clothing, platform and aspect-ratio constraints.
4. Generate **a separate complete image for each page**, including the page's short, legible text. Default to 3:4 portrait for a carousel, but honor another requested ratio. Design each page for its content rather than repeating a single layout: comparisons, sequential scenes, diagrams and moments can vary while the series remains coherent. Specify exact text, visual hierarchy, composition, character action and relevant reference roles in each image-generation request. Do not fake success with prompts, placeholders, HTML or a layered editor when the user asked for finished pictures. An image-generation tool may not expose a model name or cost; report only what is known.
5. Review the returned images themselves, including requested text and character continuity, and correct clear defects by regenerating the affected page when possible. Do not claim perfect OCR, identity or aesthetic acceptance without evidence. Preserve unaffected outputs. If a generation fails, retain completed pages, report the failed page and retry only as appropriate. User dissatisfaction with a specific page is a request to revise or regenerate that page; keep the rest.
6. Save numbered final image files in an appropriate user-accessible project folder; do not overwrite unrelated work. Provide an ordered preview and absolute local paths or a ZIP if useful, and report any material limitations. No automatic posting or publication. A completed export is not the user's aesthetic approval.

Use the host's supported choice cards when available, otherwise offer clearly labelled choices in ordinary conversation. Do not claim the Skill itself provides a graphical app or a background service. Do not publish the user's photo, character, article, or outputs unless they request that separately.
