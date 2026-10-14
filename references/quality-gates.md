# Quality gates and troubleshooting (internal)

## Before tool call

### Execution
- [ ] A real image-generation or image-edit tool is accessible; do not output a prompt instead of an image.
- [ ] The latest attached user image, not a generic stand-in, is the source.
- [ ] The user's explicitly stated revision or preferences take precedence over the standard defaults.

### Art direction
- [ ] Subject identity / recognizable IP features are accurate to what is visible or confidently known.
- [ ] A single collection concept and controlled palette unify the ten tips.
- [ ] Tip roles vary in detail density, pattern, placement and material; the quiet tips remain designed.
- [ ] At least some deliberate visual translation or micro-design is present, not a screenshot split into ten parts.
- [ ] Every dot, line, charm and symbol has a purpose.
- [ ] 3D detailing is realistic, physically proportionate and not used as an automatic marker of 'premium'.

### Render specification
- [ ] Exactly 10 detached tips in a 2×5 layout; clean top-down 1:1 photo.
- [ ] Believable curved gel surface, crisp freehand-looking line work and contact shadows.
- [ ] No text overlays, no hands, no stands, no collaged original in ordinary output.

## Review result if the host supports review and revision

- [ ] Count all ten nail tips; identify fused, cropped, duplicated or missing parts.
- [ ] Check for unwanted printed/sticker/screenshot appearance.
- [ ] Check whether recognizability survived redesign.
- [ ] Check whether auxiliary nails show designed motifs rather than meaningless dots and resin specks.
- [ ] Check dimensional embellishments do not overwhelm the art.
- [ ] Inspect for accidental lettering, watermarks or mockup props.

## User feedback → specific adjustment

| Feedback | Corrective action |
| --- | --- |
| "This looks printed" | Recompose hero motif for nail geometry, remove original pose/background/crop, switch to deliberate freehand 2D drawings. |
| "IP doesn't look right" | Correct signature geometry, facial spacing, eyes, ears, palette and distinctive accessories before adding more motifs. |
| "Too much embossing / 3D" | Reduce resin volume and props; keep the same concept while shifting detail to controlled painting, clean pattern or material contrast. |
| "Random tiny dots / no aesthetic" | Remove filler; choose one structurally meaningful pattern or clean negative space, reorganize support nails. |
| "Ten mini-scenes" | Retain a few recognizable hero nails; convert others into purposeful partial motifs, geometry and calm design. |
| "Too plain" | Strengthen one or two deliberate focal motifs, add meaningful asymmetry/pattern/material contrast rather than uniformly decorating all ten. |
| "Wrong nail count" | Regenerate or revise explicitly calling for ten separate nails in two rows of five; do not claim visual verification if absent. |
| "I wanted an example collage" | Preserve original image in top panel with a compositor, add ten-nail photo below, avoid overlay text. |

## Platform honesty

A GitHub repository does not make its skill automatically active or searchable in every AI session. The host must explicitly load/register the skill and expose uploaded image references to an actual image-generation tool. If either is missing, be honest. Do not claim a text Markdown file can bypass unavailable host tools. Quality checks improve consistency but never guarantee perfect outputs on every run.
