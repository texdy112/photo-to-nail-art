# PHOTO TO NAIL ART 💅 — v3.4 Premium Direct Image

**Upload an image → get a finished ten-piece nail-art image.** No prompt writing. No mode-selection menu. Designed for hosts with a callable image-generation tool.

**中文：**上传喜欢的照片、角色图或插画，在已加载本 Skill、且支持生图的 AI 环境中，直接生成 **10 片真实质感穿戴甲图片**。默认高级创意版，不再询问简约／复杂模式，也不会用提示词代替成品。

## Features / 功能

- **Direct image output:** while active, an image-only upload can trigger rendering; returns the real image instead of a generator prompt.
- **IP-aware direction:** recognizable character features plus thoughtful theme extension, without invented canon details.
- **Deconstruction:** nail-specific redraws, partial faces, facial details, abstract shape/pattern translation—not copied screenshots or transfer prints.
- **Art-directed 10-tip set:** designed roles, controlled palette, meaningful asymmetry, visual rhythm and small Easter eggs.
- **Craft-realistic premium style:** convincing hand painting and authentic gel texture; dimensional resin and stones only when useful.
- **Standard:** 1:1 product photo, 2 rows × 5 tips, no text, no hands or stands.
- **Optional comparison:** when specifically requested, original on top and finished ten tips below; no added labels.

## Requirements / 运行要求

This **Agent Skill is a Markdown instruction package, not a standalone image-generation app**. It cannot generate images unless the **host supports all three**:

1. Loading/activating the skill from its `SKILL.md`.
2. Passing the uploaded image reference to the assistant.
3. Calling a real image-generation / image-editing tool.

上传 GitHub 并不代表 ChatGPT、Claude、Cursor 等平台会自动发现或运行它。如果宿主平台没有生图工具，Skill 只能说明无法生成，不能凭空返回图片。

## Installation / 安装

Download the repository or ZIP, and copy the **entire `photo-to-nail-art/` folder** into the skill location supported by your host. The exact install/register step depends on the product. Ensure `SKILL.md` and `references/` stay together. Activate the skill and allow its image tool.

If uploading files through GitHub's **Upload files**, put `SKILL.md`, `README.md`, `LICENSE`, and `references/` at the repository root — **don't create a second nested folder** inside the repository. GitHub search indexing is not the same as an installed/activated skill.

## Usage / 使用方法

Once the skill is active, upload any reference image (including an image-only message). It should call the image generation tool and display a premium nail-photo result directly. Natural-language feedback like “less 3D,” “more hand-drawn,” “the character isn't accurate,” and “no screenshot-print feel” revises the result.

If you **explicitly** ask for a before-and-after case image, it should place the source image above the generated nail design below, without text overlays. This collage layout is not the default.

## Files

```text
photo-to-nail-art/
├── SKILL.md                 # Activation and image-generation contract
├── README.md                # This installation guide
├── CHANGELOG.md             # Release notes
├── LICENSE
├── .gitignore
└── references/
    ├── design-language.md  # Detailed art direction and deconstruction rules
    └── quality-gates.md    # Failure checks and revision guidance
```

## Privacy & copyright / 隐私说明

No user-uploaded reference images, private example prompts, generated test photos, chat transcripts, personal identity details or API keys are included in this public release. **The actual contents of `SKILL.md` and `references/` are public if you publish the repository publicly.** Using the skill does not itself publish your uploads to this GitHub repository; image-processing policies of the host still apply.

Third-party characters and imagery may have separate copyrights. This release licenses only its original text, not third-party artwork/IP. Review licensing before publishing any future case studies or demo images.

## Troubleshooting / 排查

**It returns only a text prompt:** the host may not have loaded the skill, or its image tool may not be available/callable. This release explicitly instructs against falling back to prompts, but cannot override platform/tool limitations.

**The repository isn't found by AI search:** give the exact URL or use the host's install mechanism. Public GitHub visibility alone does not create automatic AI skill discovery.

**Characters are printed like stickers:** the anti-transfer design gate should cause a redraw tailored to the nail, not image shrinkage.

## License

MIT for original repository contents only.
