# Programmatic Rendering — Prompt Layer

## Purpose
Translate research-derived rendering risks into explicit implementation requirements for downstream code generation.

## Determinism
For frame-by-frame rendering, all persistent procedural variation must be deterministic.
Do not use uncontrolled Math.random()-style behavior for values that must remain stable between frames.
Use seeded pseudo-random logic when procedural variation is required, with a deterministic relationship to time/frame.

## Time and frame integrity
Animation state must derive predictably from the supplied time/frame. First and last states must be reproducible.
Avoid frame-dependent accumulation that causes drift.

## Resolution independence
Use normalized/logical coordinates, responsive calculations, or scalable viewBox-like systems as appropriate so the composition can adapt without clipping or distortion.

## Typography/render readiness
If fonts are used in a renderer that loads them asynchronously, require font readiness before frame capture. Avoid layout shift between frames.

## Render performance
Keep Canvas/DOM work bounded. Avoid uncontrolled DOM/node growth, unnecessary per-frame object creation, and heavy effects that cause frame drops or corrupted output.

## Loop safety
For a loop, define exact initial/final state equivalence and deterministic return behavior. Procedural phase must not jump at the boundary.

## Technical adaptation
Apply only requirements relevant to the selected medium. Do not inject HTML/DOM rules into a Canvas-only prompt unless the source template explicitly calls for them.

## Output
Return implementation-relevant deterministic rendering constraints, not downstream code.
