# Prompt Template Builder — Layer 1

## Purpose
Take resolved commercial and creative direction and turn it into a complete production prompt while preserving the user's source template.

## No fixed production defaults
Do not assume a universal duration, scene count, aspect ratio, resolution, FPS, loop state, or other production parameter.
Every empty source field is intentionally open.
Decide values internally from the user's request, commercial use case, visual concept, medium, readability, production needs, and source knowledge.

Only values explicitly fixed by the source template remain fixed. In the active Motion Studio template, Vector and Flat vector are intentionally fixed unless the user explicitly changes them.

## Template authority
The user's supplied template is the base prompt contract.
Preserve the role statement, purpose, original section order, field names, fixed values, fixed visual rules, fixed motion rules, and fixed code/output rules.
Never shorten or silently rewrite fixed instruction blocks.

## Placeholder semantics
- An empty slot such as [ ] = infer and fill.
- An explicitly populated source value = preserve unless the user overrides it.
- An explicit user override = use the override.

## Detail mode

The builder receives one of two modes:

### Sederhana
Populate the source template and preserve its fixed content. Do not insert the extended production-specification sections.

### Full Detail
Populate the source template and insert the relevant production-specification sections needed for an implementation-ready prompt. Follow the Premium Production Prompt Specification and Motion Scene Engineering skills when applicable.

## Premium prompt expansion
A minimal base template can still produce a highly detailed professional prompt through generated production-specification sections.

For the active Motion Studio prompt, preserve the original settings/concept fields and insert generated production detail before the original fixed ATURAN VISUAL, ATURAN MOTION, and ATURAN KODE blocks.

Preferred sections for a non-trivial motion prompt:
1. DESKRIPSI
2. Konsep Visual
3. Style
4. Palet Warna
5. Struktur Scene / Scene Flow
6. Timeline Motion
7. Detail Motion Language
8. Camera & Composition
9. Keyframe Summary
10. Easing Recommendation
11. Overall Art Direction
12. Technical Production Direction when materially relevant

## Fidelity rule
Generated enrichment may expand the source prompt but must not replace, delete, reorder, summarize, or weaken its fixed blocks.
The template's downstream instructions are content being assembled. Layer 1 must not execute them.

## Detail standard
Each generated section must contain concrete information useful to a downstream code generator.
Prefer state descriptions, spatial relationships, timing ranges, meaningful motion values/ranges, easing behavior, color roles, and implementation-relevant constraints over vague adjectives.

Do not pad the prompt merely to make it longer.

## Final output
The result is one complete ready-to-use production prompt.
Never generate the downstream JavaScript, HTML, SVG, image, or MP4.
