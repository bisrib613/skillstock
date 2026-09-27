# Programmatic Rendering

For Canvas, SVG, and HTML/browser-rendered motion.

## Determinism
Never rely on uncontrolled randomness for persistent frame-to-frame elements. Use seeded pseudo-random values tied to stable IDs and/or frame/time.

## Resolution independence
Use normalized/logical coordinates or scalable viewBox systems.

## Frame safety
Ensure:
- first frame is valid
- font loading is synchronized before capture when fonts are used
- no layout shift
- no uncontrolled asynchronous asset arrival
- deterministic timing
- bounded Canvas/DOM work
- no per-frame DOM explosion

## Loops
Make initial and final visual states connect exactly when a seamless loop is requested.

Preview behavior and final frame-by-frame encoding are not assumed to be identical.