# Listing Copy and Starter Prompts — Mixmatter 2.1

## Info

### Plugin name

`Mixmatter`

### Short description

`AI art direction for existing imagery`

### Long description

Mixmatter 2.1 turns a user-supplied image into a source-aware contemporary print reconstruction by combining art-direction judgment with the established Mixmatter visual language.

It reads the source before transforming it: identifying semantic anchors, visual hierarchy, structural relations, identity invariants, low-information fields, clutter, and transformation opportunities. It then decides what must be preserved, what may be transformed or removed, and forms one dominant source-specific direction thesis.

The reconstruction prioritizes structural operations such as crop, isolation, suppression, scale contrast, planar compression, controlled fragmentation, and overlap before material effects. Halftone, duotone, torn or cut edges, paper layering, registration shifts, and photocopy-like behavior are used selectively when they reinforce hierarchy, separation, rupture, compression, or artifact-ness.

> **Photography is source material, not sacred material.**
>
> **Reconstruct, do not decorate.**
>
> **Preserve semantic identity, not visual completeness.**

Clear requests execute directly. For vague requests, Mixmatter inspects the source and chooses the strongest source-specific direction by default. It asks for clarification or offers alternatives only when multiple plausible readings would materially change the result.

Revisions preserve successful crop, hierarchy, explicit locks, identity-bearing details, and useful material decisions rather than restarting from a random composition. If the user asks for a new alternative from the original source, Mixmatter returns to that original source unless instructed otherwise.

Mixmatter 2.1 adds zero new text by default. Existing source text remains in its original language and may be preserved selectively when it matters to identity. It is not translated or duplicated into a bilingual layout by default. If exact source text cannot be reproduced reliably, it should be obscured, cropped, simplified, or treated as source texture rather than replaced with hallucinated wording. New wording is used only when the user supplies it exactly or explicitly authorizes generated copy.

Mixmatter is designed for existing imagery. It is not a generic style marketplace, broad photo editor, cinematic realism engine, or from-scratch design suite.

Typical sources include:

- cities, streets, architecture, transport, and infrastructure
- landscapes, interiors, and public spaces
- portraits, people, and animals
- food, objects, retail environments, and cultural artifacts

Mixmatter does not operate a separate image-generation backend or require an MCP service. Image understanding and generation/editing are performed by the host platform when available.

### Category

`Creativity`

### Publisher

- Public publisher brand: `Galok`
- Developer: `Fan Jiale`, an individual developer publishing under the Galok brand
- Verified developer identity: `Fan Jiale`

### Version

`2.1.0`

### Public URLs

- Website: `https://www.galok.me/mixmatter/`
- Support: `https://www.galok.me/mixmatter/support/`
- Privacy policy: `https://www.galok.me/mixmatter/privacy/`
- Terms of use: `https://www.galok.me/mixmatter/terms/`

## Starter prompts

1. `Process this image with Mixmatter. Preserve what makes the source identifiable and do not add new text.`
2. `Make this image flatter and more graphic with Mixmatter. Preserve the main subject and defining structure.`
3. `Reconstruct this portrait with Mixmatter. Keep the identity intact, simplify the background, and add no new typography.`

## Prompt intent

The three prompts test autonomous default judgment, stronger graphic reconstruction, and portrait preservation.

All starter prompts assume that the user attaches a source image. Mixmatter uses host image understanding and image generation/editing when those capabilities are available; it does not operate a separate image-generation backend or custom host UI.
