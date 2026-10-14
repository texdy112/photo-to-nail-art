---
name: photo-to-nail-art
description: >-
  Create an actual premium 10-piece press-on nail image from a user-uploaded photo,
  illustration, or IP character. While this skill is active, even an image-only
  upload triggers direct image generation when the host supports it. No prompt-only
  output, no simple/complex selection, no printed-photo nails. Use for image-to-nail,
  nail-art redesign, and follow-up revisions.
---

# PHOTO TO NAIL ART v3.4 — Premium Direct Image

## 1. First obligation: create the image, not a prompt

**This is an IMAGE-IN → IMAGE-OUT skill. Its normal deliverable is a rendered image.**

When this skill is active and the user supplies a reference image — including an **image-only message without text** — directly produce a premium nail-art design. The image upload alone is sufficient to start; do not ask whether the user prefers simple or complex. Use the **latest user-provided reference**, unless the user identifies another one.

Execute in this order:
1. Inspect the actual uploaded reference and determine the visual subject and user preferences.
2. Silently develop and edit one coherent ten-tip nail design using the rules below and the two files in `references/`.
3. **Call the host's actual available image-generation or image-editing tool**. Supply the uploaded image by its supported attachment/reference mechanism. Ask it to render the finished product photograph; do not merely construct a text prompt for the user.
4. Display the **actual generated image** as the result. For ordinary image requests, do not preface it with planning notes, a design breakdown, copied prompts or other filler.

**Never substitute a prompt, design list, Markdown image link, or imagined generated-image URL for a real tool call.** If the host cannot access an image generator, state briefly that this environment cannot render the result; do not return a prompt unless the user explicitly asks for one. If generation fails, report that fact rather than claiming success.

When the user explicitly asks to explain, edit the skill itself, produce prompts, audit a repository, or perform another non-image task, follow that request rather than rendering unsolicited nail images. A standalone GitHub repository does not automatically install or activate a skill in every AI chat.

## 2. Creative direction: premium, not overloaded

Act as a professional nail-art creative director and practical nail technician. Create **a collection**, not ten mini-prints of the reference.

- **Identify accurately.** Read subject, recognizable character/IP where clear, signature facial geometry, palette, accessories, form, era and mood. Never hallucinate official lore or treat invented decoration as canonical IP detail.
- **Consider a visual world.** Distinguish (a) genuinely visible/certain IP attributes, (b) defensible related props and motifs, (c) optional independent stylistic extensions. Do not inject Y2K, bows, stars or candy colors by habit.
- **Choose a collection concept.** Silently compare a few distinct art directions; select the strongest. The concept guides motif, palette, texture, visual hierarchy and craft. Do not invent a concept only after assembling random decorations.
- **Deconstruct, do not transfer.** Translate source features into nail-specific drawings and graphics: partial faces, peeking ears, face details, paw silhouettes, accessories, bold shape boundaries, French curves, deliberate lines, structured dots/checks/stripes or theme-specific geometry. Change framing to fit the nail's long, curved shape.
- **Compose ten intentional roles.** Vary recognizable hero art, meaningful symbols, patterns where relevant, carefully chosen material looks and designed quiet tips. Use variety without enforcing rigid quotas. Supporting tips must still look purposeful on their own.
- **Include micro-design selectively.** Think cropped/offset faces, edge-peeking details, detached expressive marks, asymmetric placement and one or two memorable surprises. Not every nail requires a tiny extra.
- **Let craft follow design.** Finely hand-painted 2D characters are often right; subtle raised gel, syrup gel, cat-eye, shimmer and tiny gems are optional. Creative/premium does **not** mean covering every tip in oversized 3D sculpture.

Use `references/design-language.md` for the expanded art-direction heuristics, and `references/quality-gates.md` for failure patterns and corrective decisions.

## 3. Nonnegotiable anti-transfer / anti-filler rules

**Never copy, shrink, crop, print, paste or transfer an uploaded photograph, cartoon frame, poster, screenshot or full scene straight onto a nail.** A hero character may be recognizable or even fully represented **only when redrawn and recomposed specifically for the nail**, without the original screenshot framing, foreground/background baggage or rectangular poster aesthetic.

Avoid:
- Miniature original images or pseudo-sticker prints on the nail.
- All-ten continuous landscapes or ten repeated front-facing portraits.
- Random decorative specks, stray dashes, unstructured dots, scatter stars, filler hearts or gratuitous waterdrops.
- Generic unrelated props selected only because they are trendy.
- Too many large resin charms or thick toy-like 3D characters.

Pattern quality matters: gingham/checks must be an actual ordered grid; polka dots need rhythm and scale; stripes need intentional width/placement. Sometimes the best edit is **removing** an unnecessary element.

## 4. Mandatory standard output specification

Invoke image generation to produce:

- **ONE square (1:1), photorealistic nail-product photograph**.
- **EXACTLY ten separate, detached press-on nail tips in two rows of five**, entirely visible, neatly and evenly spaced.
- Consistent medium oval/almond tip shapes unless the user specifies another shape.
- Clean neutral warm-white/cream or soft light-gray background, top-down view, believable scale, natural contact shadows and subtle optical highlights on real curved gel.
- Distinct, coherent nail designs with crisp hand-painted details. Two-dimensional cartoon drawing **on a real glossy nail** is welcome; a flat digital illustration of ten nails is not.
- Only plausible nail materials and construction; no giant overhanging parts, fused tips or floating ornaments.
- **NO extra text of any kind within the image**: no captions, overlay labels, logos, watermarks, mockup interface, digits, decorative lettering, arrows or title. No fingers, mannequin hands, boxes, nail stands, trays or photography props.

**Default: just the 10-tip image, not a collage.** Respect explicit user overrides where feasible. If image-generation tooling supports revision/inspection and results violate critical constraints, fix and regenerate within available limits. Do not promise perfect 10-tip counting or guaranteed IP fidelity.

## 5. Special case: original-above / nail-art-below comparisons

**Only when explicitly asked** for a before/after or example collage, create a vertical two-panel result: **upper = the user's actual original image; lower = the newly generated ten-tip photo**. Include no added text, arrows or logos. To keep the original pixel-faithful, compose the actual uploaded image and finished generated nail photo using an image compositing tool if the host provides one. If exact original-image inclusion cannot be achieved, disclose that limitation rather than pretending the recreated upper panel is exact. An ordinary image upload must not trigger this collage layout.

## 6. Revisions and honest limitations

For requests such as “less 3D,” “more hand-painted,” “not recognizable,” “too much print transfer,” or “no aesthetic,” regenerate using the original reference while updating only the criticized dimension. Diagnose and **redesign**, not just add embellishments.

Do not save, publish, or embed the user's uploaded images or private example prompts into a public repository. Output and image-processing privacy depend on the host platform's own policies. The skill is a written workflow, not an image model or autonomous upload listener.
