# Programmatic Rendering — Prompt Layer

## Purpose
Translate research-derived rendering risks into explicit implementation requirements for downstream code generation.

## Determinism
For frame-by-frame rendering, persistent procedural variation must be deterministic.
Avoid uncontrolled Math.random()-style values for persistent state.
Use seeded pseudo-random logic when procedural variation is needed, with a deterministic time/frame relationship.

## Time and frame integrity
Animation state must derive predictably from supplied time/frame. First and last states must be reproducible. Avoid frame-dependent accumulation that causes drift.

## Resolution independence
Use normalized/logical coordinates, responsive calculations, or scalable viewBox-like systems as appropriate so the composition adapts without clipping or distortion.

## Typography/render readiness
If fonts load asynchronously, require font readiness before frame capture. Avoid layout shift between frames.

## Render performance
Keep Canvas/DOM work bounded. Avoid uncontrolled node growth, unnecessary per-frame object creation, and heavy effects that cause frame drops or corrupted output.

## Loop safety
Define exact initial/final state equivalence and deterministic return behavior. Procedural phase must not jump at the boundary.

## Technical adaptation
Apply only requirements relevant to the selected medium. Do not inject HTML/DOM rules into a Canvas-only prompt unless the source template requires them.

## Output
Return implementation-relevant deterministic rendering constraints, not downstream code.
