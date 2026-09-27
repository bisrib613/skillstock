# Premium Production Prompt Specification — Layer 1

## Purpose
Convert commercial intelligence and art direction into the depth of specification required for a professional downstream production prompt.

## Target quality
The reference quality target is an implementation-ready production specification, not merely a theme, style label, and generic motion instructions.

Use the depth of a professional motion brief as the target, while adapting technical rules to the selected medium.

## Specification stack
For a non-trivial motion prompt, define as applicable:
1. Commercial purpose / communication goal
2. Conceptual situation
3. Visual system
4. Subject and state hierarchy
5. Composition and framing
6. Background/environment support
7. Scene/state architecture
8. Exact timeline
9. Primary motion
10. Secondary and micro movement
11. Transition behavior
12. Keyframe checkpoints
13. Easing and velocity character
14. Color roles and palette
15. Typography behavior when relevant
16. Camera/viewport behavior
17. Loop strategy
18. Technical production direction
19. IP/asset restrictions

Do not force every layer into every prompt. Select the layers required by the concept.

## No production defaults
Do not assume duration, scene count, aspect ratio, resolution, FPS, or loop state from a previous example.
Decide these internally from explicit user constraints first, then from commercial use, concept complexity, readability, renderer needs, and loop requirements.

## Detail is operational
Translate abstract adjectives into concrete attributes.

Examples:
- premium → controlled hierarchy, spacing, restrained effects, deliberate motion, coherent surfaces
- dynamic → identify the object, action, timing, acceleration/deceleration, and settling
- clean → specify spacing, object separation, contrast, and absence of clutter
- modern UI → specify surface language, component geometry, interaction state, and depth behavior

## Timeline standard
When duration is known or inferred, cover the full runtime from 0.00s to the selected end.
Use meaningful ranges rather than disconnected timestamps.
Represent entrance, primary action, state transition, hold, and ending/loop preparation when applicable.

## State architecture
Build animation around meaningful visual states.
A typical sequence might be initial → interaction → processing → resolution → hold → return/loop, but adapt it to the actual concept.

## Keyframe standard
Important checkpoints should communicate time, state, primary motion, and supporting motion.
Keyframes are checkpoints, not a substitute for the full timeline.

## Easing standard
Map easing to behavior. Use named easing families or concrete cubic-bezier values when useful. Do not add arbitrary values without a visual reason.

## Composition standard
For important subjects, define relative placement, scale hierarchy, visual focus, margins/safe areas, depth relationships, and background support.
Do not use a copy-space percentage as a universal rule. Apply copy space only when the buyer/use case benefits from it.

## Palette standard
When color is important, define functional roles such as background, surface, primary, secondary, accent, success/warning, text, shadow, and highlight.
Choose a coherent limited system appropriate to the concept.

## Technical adaptation
Separate creative specification from renderer-specific implementation.
For Canvas/JavaScript prompts, preserve Canvas-only constraints and express technical direction through responsive coordinates, deterministic time-based animation, render-safe drawing, and loop-safe state logic.
Do not copy HTML/CSS-specific implementation rules into a Canvas prompt unless the source template explicitly requires them.

## Restraint
Premium detail does not mean maximal complexity. Do not add particles, lighting, camera movement, UI elements, text, or numerical parameters unless they improve comprehension, polish, commercial utility, or implementation clarity.