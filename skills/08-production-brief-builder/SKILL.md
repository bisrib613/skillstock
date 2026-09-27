# Prompt Template Builder — Layer 1

## Purpose

Take the resolved commercial and creative direction and turn it into a complete production prompt while preserving the user's source template.

## Template authority

The user's supplied template is the base prompt contract.

Preserve:
- role statement
- purpose
- original section order
- field names
- populated defaults
- fixed visual rules
- fixed motion rules
- fixed code/output rules

Never shorten or silently rewrite the user's fixed instruction blocks.

## Placeholder semantics

- `[ ]` or another intentionally empty slot = infer and fill.
- A populated default such as `[10 detik]`, `[2 scene]`, `[16:9]`, `[Vector]`, or `[Flat vector]` = preserve unless explicitly overridden.
- A user-provided override = use the override.

## Premium prompt expansion

A minimal base template can still produce a professional prompt when the builder adds the missing creative specification around it.

For the active Motion Studio prompt, the builder should preserve the original settings and then generate a detailed production specification before the original fixed ATURAN VISUAL, ATURAN MOTION, and ATURAN KODE blocks.

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

The source template's own KONSEP VISUAL field remains intact. Generated Concept Visual detail may expand its meaning but must not overwrite the source's fixed wording.

## Expansion quality

Every generated section must answer an implementation question.

### DESKRIPSI
State the communication goal, subject, user/system flow, and visual situation.

### KONSEP VISUAL
Describe the main visual system and the sequence of meaningful states.

### STYLE
Translate the requested style into concrete surface, shape, lighting, depth, and restraint characteristics.

### PALET WARNA
Assign functional color roles such as background, surface, primary, success/warning, text, shadow, and highlight when relevant. Keep the palette coherent and theme-appropriate.

### STRUKTUR SCENE
Describe the state/action sequence. Avoid scenes that exist only for decoration.

### TIMELINE MOTION
Give exact or approximate time ranges that cover the entire declared duration. Include meaningful beats, transitions, and holds.

### DETAIL MOTION LANGUAGE
Specify interaction behavior, micro-motion, acceleration/deceleration, settling, and secondary motion where useful.

### CAMERA & COMPOSITION
Define framing, focal placement, scale hierarchy, safe areas, depth, and background support elements when relevant.

### KEYFRAME SUMMARY
Summarize the critical state changes at useful timestamps.

### EASING RECOMMENDATION
Map easing behavior to actions instead of applying one generic easing to everything.

### OVERALL ART DIRECTION
Close the creative loop with the intended visual character, commercial utility, and important anti-generic constraints.

## No padding

Do not add detail merely to increase prompt length.

Do not copy the entire research report into the prompt.

Do not invent unsupported factual claims.

Do not create arbitrary technical numbers with no production purpose.

## Layer boundary

The result of this skill is a complete prompt only.

Never generate JavaScript, HTML, CSS, SVG code, MP4, or downstream assets.

## Final QA

Before returning:
- resolve required placeholders
- preserve populated defaults
- preserve fixed template rules
- confirm timeline continuity
- confirm internal consistency
- confirm premium specification depth
- confirm the result is still a prompt, not generated code.

## Field discipline
Keep settings fields concise and semantically clean. Do not stuff long narrative into TEMA VIDEO or other single-value fields merely to increase detail. Put implementation detail into the generated production-specification sections.