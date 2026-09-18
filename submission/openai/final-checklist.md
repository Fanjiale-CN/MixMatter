# Final Submission Readiness Checklist — Mixmatter 2.1

This checklist covers the UI-independent Skills-only Mixmatter 2.1 package.

## Repository readiness

- [x] Public product name is `Mixmatter`.
- [x] Package version is `2.1.0`.
- [x] Portable manifest is present at root `plugin.json`, including OpenAI-specific listing metadata under `extensions.com.openai.interface`; `.codex-plugin/plugin.json` remains as a compatibility fallback.
- [x] Packaged Skill is present at `skills/mixmatter/`.
- [x] Packaged references include `mixmatter-v1.md`, `mixmatter-v2-runtime.md`, and `quality-rubric.md`.
- [x] The seven canonical research/system outputs are retained.
- [x] ChatGPT host UI source code has been removed from the active product architecture.
- [x] Host-UI specification documents have been removed from the active product architecture.
- [x] The Skill no longer depends on creation/result cards, widgets, or MCP UI tools.
- [x] Direction / Structure / Intensity remain available as natural-language product semantics.
- [x] Revision continuity remains part of the 2.1 behavior.
- [x] Source-text protection remains strict.
- [x] Light and dark Mixmatter icon assets are present.
- [x] Privacy and Terms describe a Skills-only architecture with no separate Mixmatter MCP service.

## Behavior checks

- [ ] Re-test default vague invocation with representative source images.
- [ ] Confirm vague requests produce autonomous source-specific judgment rather than a menu or generic preset list.
- [ ] Confirm explicit requests execute directly.
- [ ] Confirm a revision preserves successful crop, identity, hierarchy, locks, and useful material decisions.
- [ ] Confirm an alternative-from-source returns to the original source image unless the user requests otherwise.
- [ ] Confirm default results are visibly reconstructed rather than ordinary photo styling.
- [ ] Confirm material effects remain selective and causally justified.
- [ ] Confirm zero new text is added by default.
- [ ] Confirm uncertain source text is obscured/cropped rather than hallucinated.
- [ ] Confirm source text is not translated or bilingual-duplicated by default.
- [ ] Run representative cases from `docs/system/MIXMATTER_REGRESSION_BENCHMARK.md`.

## Submission package

The final ZIP should preserve this relevant structure:

```text
plugin.json
skills/
└── mixmatter/
    ├── SKILL.md
    └── references/
        ├── mixmatter-v1.md
        ├── mixmatter-v2-runtime.md
        └── quality-rubric.md

assets/
├── mixmatter-icon-light.svg
└── mixmatter-icon-dark.svg
```

Do not include the retired `apps/mixmatter-chatgpt/` implementation as an active runtime dependency.

## Review materials

- [x] 2.1 listing copy prepared.
- [x] Three 2.1 starter prompts prepared.
- [x] Positive and negative review-test framework prepared.
- [x] 2.1 release notes prepared.
- [x] Public website, support, privacy, and terms URLs are listed.
- [x] Developer / publisher relationship remains `Fan Jiale` / `Galok`.

## Portal actions

- [ ] Build the final Plugin ZIP from the reviewed repository state using the `Build Mixmatter OpenAI Package` workflow.
- [ ] Upload that exact ZIP to the OpenAI submission flow.
- [ ] Confirm the portal parses root `plugin.json` successfully; root `extensions.com.openai.interface` is the authoritative OpenAI listing configuration.
- [ ] Copy the finalized listing details and starter prompts.
- [ ] Add the positive and negative tests from `test-cases.md`.
- [ ] Confirm country / region availability at submission time.
- [ ] Review all policy attestations before submission.

## Go / no-go status

**Status: MIXMATTER 2.1 PACKAGE STRUCTURE READY; AUTOMATED ZIP BUILD + PORTAL UPLOAD PENDING.**
