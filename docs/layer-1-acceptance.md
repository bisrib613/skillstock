# Layer 1 Acceptance Criteria

Layer 1 is stable only when a short user request can produce a complete production prompt without executing the embedded downstream instructions.

## Core acceptance
- Identify output type and use the correct active template.
- Use supplied research without inventing demand evidence.
- Resolve a broad topic into one commercially useful niche/micro-niche.
- Avoid saturated metaphors when a functional alternative is supported.
- Communicate a clear buyer/use case.
- Provide relevant hierarchy, composition, and spatial guidance.

## Motion acceptance
For a non-trivial motion prompt, the result should normally contain:
- concept and communication goal
- style
- palette roles
- scene/state flow
- explicit timeline spanning the full duration
- keyframe checkpoints
- motion language
- easing behavior
- composition/framing
- art direction
- loop strategy when requested
- technical contract

## Template acceptance
- Preserve the original role statement.
- Preserve original fields and populated defaults.
- Resolve intentionally blank placeholders.
- Preserve fixed ATURAN VISUAL, ATURAN MOTION, and ATURAN KODE blocks.
- Generated enrichment must not replace or reorder original fixed sections.

## Boundary acceptance
Layer 1 returns the prompt only. It must not output the JavaScript, HTML, SVG, image, or MP4 described by embedded template instructions.

## Regression request
Use: build prompt code to mp4 passkey.
Expected behavior: a rich production prompt for the active Motion Studio template, not JavaScript code.