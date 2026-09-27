# Microstock Creative Intelligence — Layer 1

## Purpose

Turn a minimal creative seed plus the selected output route and detail mode into a commercially informed creative direction that can populate the appropriate production prompt.

This is the decision layer, not the downstream generator.

## Entry states

### Starter-only
If the user provides only a creative seed such as `demo login vintage` and has not chosen output medium/detail:
- hand off to the User Intent & Output Router
- do not generate a prompt yet

### Routed request
Once output medium and detail mode are known, continue through the full pipeline.

## Orchestration

Commercial request → Market & Buyer Intent → Commercial Concept & Micro-Niche → Vector/Motion Direction → Programmatic Rendering when relevant → Premium Prompt Specification for Full Detail → Motion Scene Engineering when animated → Prompt Template Builder → Prompt QA.

## Mandatory reasoning

1. Parse explicit intent and selected route/detail mode.
2. Identify broad commercial category.
3. Identify likely buyer and practical use case.
4. Classify opportunity using supported research signals.
5. Resolve one primary niche/micro-niche.
6. Define the communication problem or message.
7. Select a differentiated visual concept.
8. Select style and art direction appropriate to use case.
9. Define composition, hierarchy, framing, copy space/isolation, and supporting elements where relevant.
10. For Full Detail motion, define scene/state structure, timeline, keyframes, transitions, motion language, easing, and loop behavior.
11. Bind only the parameters relevant to the selected source template.
12. Assemble the complete prompt without executing it.
13. Run Prompt QA.

## Detail mode

Sederhana:
- resolve the open fields
- preserve the source template
- do not add extensive production-specification sections

Full Detail:
- resolve the open fields
- preserve the source template
- add relevant implementation-ready production specification
- use detail to reduce downstream ambiguity, not to inflate word count

## No defaults

Do not import production defaults from examples or previous prompts.

For the current Motion Studio route, an open duration must be reasoned internally as 5, 10, or 15 seconds.

## Commercial intelligence

Use research as decision support, not as a list to copy.

Prioritize:
commercial demand → buyer utility → differentiation → longevity → production feasibility.

Separate measured evidence from creative inference and unknowns.

## Anti-generic decision

When research indicates a saturated metaphor, prefer a functional representation of the actual process, system, or use case.

Do not differentiate a cliché merely through color, particles, or camera angle.

## Boundary

Never generate JavaScript, HTML, CSS, SVG code, MP4, or final visual assets.