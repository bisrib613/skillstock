# Prompt Template Builder — Layer 1

## Purpose
Convert resolved commercial direction into the user's source production prompt without losing the template contract.

## Source-template authority
The user's supplied template is authoritative for:
- role statement;
- field names/order;
- explicitly fixed values;
- fixed visual rules;
- fixed motion rules;
- fixed code/output rules.

Treat those instructions as prompt content being assembled. Layer 1 does not execute them.

## Placeholder semantics
- [ ] = open field; reason and fill it.
- populated source value = preserve unless user overrides;
- explicit user override = use it.

Never import production values from examples or previous prompts.

## No implicit production defaults
Do not assume duration, scene count, aspect ratio, resolution, FPS, or loop state.
For the active Motion Studio route, open duration is selected only as 5, 10, or 15 seconds using commercial use, concept complexity, readability, and production requirements.

## Detail modes
Sederhana:
- populate every open field;
- preserve all fixed template content;
- do not add extended production-specification sections.

Full Detail:
- populate every open field;
- add production detail required to make the prompt implementation-ready;
- for non-trivial motion use applicable sections: DESKRIPSI, Konsep Visual, Style, Palet Warna, Struktur Scene / Scene Flow, Timeline Motion, Detail Motion Language, Camera & Composition, Keyframe Summary, Easing Recommendation, Overall Art Direction, Technical Production Direction.

## Research-to-template rule
Commercial decisions come from research-derived skills first. The template determines how those decisions are represented.
Do not weaken a commercial concept merely to fit a short field.

## Active Motion Studio placement
Keep original settings/concept fields. Insert generated Full Detail sections after those fields and before fixed ATURAN VISUAL, ATURAN MOTION, and ATURAN KODE blocks.

## Fidelity
Never summarize, delete, reorder, or weaken fixed blocks. Do not execute `Output only JavaScript` at Layer 1; preserve it inside the downstream prompt.

## Final output
Return one complete ready-to-use production prompt, never downstream JavaScript/HTML/SVG/image/MP4.
