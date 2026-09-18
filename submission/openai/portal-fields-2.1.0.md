# OpenAI Plugin Submission — Matter 2.1.0

This file is the final copy sheet for the OpenAI submission portal. It does not change the current ChatGPT plugin identity.

## Submission type

Skills only.

No MCP server, external account, authentication, demo credentials, or separate image-generation backend is required.

## Information

**Plugin name:** Matter

**Short description:** AI art direction for existing imagery

**Category:** Creativity

**Developer identity:** Fan Jiale

**Publisher brand:** Galok

**Website:** https://www.galok.me/press-print/

**Support:** https://www.galok.me/press-print/support/

**Privacy policy:** https://www.galok.me/press-print/privacy/

**Terms:** https://www.galok.me/press-print/terms/

**Repository:** https://github.com/Fanjiale-CN/press-print

## Long description

Matter 2.1 turns a user-supplied image into a source-aware contemporary print reconstruction by combining art-direction judgment with the established Matter visual language.

It reads the source before transforming it: identifying semantic anchors, visual hierarchy, structural relations, identity invariants, low-information fields, clutter, and transformation opportunities. It then decides what must be preserved, what may be transformed or removed, and forms one dominant source-specific direction thesis.

The reconstruction prioritizes structural operations such as crop, isolation, suppression, scale contrast, planar compression, controlled fragmentation, and overlap before material effects. Halftone, duotone, torn or cut edges, paper layering, registration shifts, and photocopy-like behavior are used selectively when they reinforce hierarchy, separation, rupture, compression, or artifact-ness.

Clear requests execute directly. For vague requests, Matter inspects the source and chooses the strongest source-specific direction by default. Revisions preserve successful crop, hierarchy, explicit locks, identity-bearing details, and useful material decisions instead of restarting from a random composition.

Matter adds zero new text by default. Existing source text remains in its original language and may be preserved selectively when it matters to identity. It is not translated or duplicated into a bilingual layout by default. If exact source text cannot be reproduced reliably, it should be obscured, cropped, simplified, or treated as source texture rather than replaced with hallucinated wording. New wording is used only when the user supplies it exactly or explicitly authorizes generated copy.

Matter is designed for existing imagery. It is not a generic style marketplace, broad photo editor, cinematic realism engine, or from-scratch design suite.

## Starter prompts

1. Process this image with Matter. Preserve what makes the source identifiable and do not add new text.
2. Make this image flatter and more graphic with Matter. Preserve the main subject and defining structure.
3. Reconstruct this portrait with Matter. Keep the identity intact, simplify the background, and add no new typography.

## Five positive test cases

### P1 — Vague invocation / autonomous judgment

**Prompt:** Process this image with Matter.

**Fixture:** Attach a non-sensitive street, city, interior, object, or landscape image.

**Expected:** Matter reads the actual source, identifies semantic and structural anchors, forms a source-specific direction, visibly reconstructs the composition, and introduces no new text by default.

### P2 — Explicit strong reconstruction

**Prompt:** Make this flatter and more graphic with Matter. Preserve the main subject and defining structure. No new text.

**Fixture:** Attach a non-sensitive architecture, transport, streetscape, or public-space image.

**Expected:** Execute directly. Use structural operations such as crop/reframe, planar compression, isolation, suppression, or scale contrast before decorative texture. Preserve identity-bearing structure.

### P3 — Portrait preservation

**Prompt:** Reconstruct this portrait with Matter. Keep the identity intact, simplify the background, and add no new typography.

**Fixture:** Attach a non-sensitive portrait the reviewer has permission to use.

**Expected:** Protect face identity, decisive pose/gesture, and important subject relationships while spending redundant background detail first.

### P4 — Dense source signage

**Prompt:** 用 Matter 重构这张街景。保留场景身份，但不要新增、翻译或双语复制任何文字。

**Fixture:** Attach a non-sensitive metro, railway, storefront, or commercial-street image with visible signage.

**Expected:** Preserve identity-critical source wording when feasible; crop, fragment, obscure, or reduce secondary text. Do not translate, create bilingual duplicates, invent replacement wording, or add filler editorial copy.

### P5 — Revision continuity

**Prerequisite:** Create a successful Matter result from any suitable source.

**Prompt:** Keep this crop and the subject treatment. Reduce the tearing and make the right side quieter.

**Expected:** Preserve successful crop, identity, hierarchy, locks, and useful material decisions. Change the requested axis instead of rerolling the composition.

## Three negative test cases

### N1 — Faithful restoration without Matter intent

**Prompt:** Restore this old photograph naturally and faithfully.

**Expected:** Matter should not be selected automatically. Faithful archival-style restoration is outside the core reconstruction workflow.

### N2 — Unrelated watercolor conversion

**Prompt:** Turn this image into a watercolor painting.

**Expected:** Matter should not be selected automatically because the request asks for a different transformation language.

### N3 — From-scratch typography-heavy design

**Prompt:** Design a typography-heavy exhibition poster from scratch with a large headline, date, and editorial body copy.

**Expected:** Matter should not be selected automatically. Its core identity is source-image art direction and reconstruction rather than a generic from-scratch typesetting suite.

## Release notes

### Matter 2.1.0

- adds hierarchy stabilization for diffuse, repetitive, sparse, or ambiguous sources;
- organizes repeated subjects into dominant, supporting, and field roles when appropriate while preserving group identity;
- assigns substantial low-information fields explicit compositional jobs rather than filling them arbitrarily;
- strengthens source-specific art-direction judgment, revision continuity, and source-text protection;
- retains the Skills-only, UI-independent architecture with no MCP server or external authentication requirement;
- keeps the established Matter visual language authoritative while improving structural decision quality.

## Reviewer setup

Attach any non-sensitive source image the reviewer has permission to use. No demo credentials, MFA, SMS, email confirmation, private-network access, test account, external API key, or Matter backend is required.

## Availability

Select the countries and regions you intend to support in the OpenAI submission portal where the relevant host image capabilities are available. The package itself has no region-specific backend, account system, payment provider, or external data service.
