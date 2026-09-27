# SkillStock

Repository for a reusable **Layer 1 microstock prompt-generation system**.

## Current scope

The current build stops at **FINAL PROMPT**.

It does not generate JavaScript, HTML, CSS, SVG code, MP4, or downstream production files yet. Layer 2 is intentionally deferred.

## Current flow

Short user command
→ commercial/creative reasoning
→ choose applicable prompt template
→ fill only intentionally open fields
→ preserve fixed template content and defaults
→ prompt QA
→ final ready-to-use production prompt

## User experience

The user should be able to use short commands such as:

- `build prompt code to mp4`
- `build prompt motion passkey`
- `build prompt mobile car sharing`

The system should infer commercially useful context from the supplied research and skills instead of making the user complete a long form.

## Template fidelity

A user-supplied template is the authoritative base prompt.

- Preserve its role statement and purpose.
- Preserve section order and field names.
- Preserve populated defaults unless the user explicitly overrides them.
- Fill intentionally blank placeholders from research/skills.
- Preserve all fixed visual, motion, and code rules.
- Do not shorten, summarize, or redesign the template.
- Do not add unrelated fields.
- Do not generate the downstream code in Layer 1.

## Architecture

- `research/` — research-derived operational knowledge
- `skills/` — reasoning and prompt-building skills
- `templates/` — prompt templates
- `system-instructions/` — platform-specific Layer 1 instructions

## Commercial principle

commercial demand → buyer utility → differentiation → longevity → production feasibility

Do not invent unsupported sales data, marketplace guarantees, search-ranking weights, or moderation thresholds.