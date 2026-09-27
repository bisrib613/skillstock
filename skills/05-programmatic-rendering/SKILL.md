# Programmatic Rendering — Prompt Layer

## Purpose
Translate rendering constraints into explicit prompt instructions for downstream code generation.

## Determinism
For frame-by-frame rendering, require deterministic procedural behavior.
Avoid uncontrolled randomness that changes persistent positions or states between frames.
Use seeded pseudo-random values when procedural variation is needed.

## Resolution independence
Use normalized/logical coordinates, responsive layout calculations, or scalable viewBox systems as appropriate.

## Frame safety
Prompt requirements should cover valid first frame, deterministic timing, no layout shift, font readiness before capture when fonts are used, bounded Canvas/DOM work, no uncontrolled asynchronous dependencies, and no per-frame DOM explosion.

## Loop safety
When looping, define the initial state, final state, return path, and deterministic loop endpoints.

## Renderer awareness
Do not assume interactive browser preview and frame-by-frame encoded output behave identically.
Prompt the downstream generator to optimize for deterministic rendering rather than only interactive appearance.

## Output
Return technical requirements relevant to the selected output template. Do not inject unrelated renderer technologies.