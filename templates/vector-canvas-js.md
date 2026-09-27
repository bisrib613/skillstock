# Vector / Canvas JavaScript Production Template

Role: professional vector designer + JavaScript Canvas developer for premium commercial microstock.

THEME: [theme]
COMMERCIAL CATEGORY: [category]
MICRO-NICHE: [micro-niche]
BUYER / USE CASE: [buyer]
DURATION: [duration]
SCENES: [scene count]
ASPECT RATIO: [ratio]
VISUAL STYLE: [style]
CONCEPT: [concept]
COMPOSITION: [composition]
HIERARCHY: [hierarchy]
COPY SPACE / ISOLATION: [strategy]
COLOR: [palette]

## Visual
Premium, modern, professional, commercial. Clear focal point and hierarchy. Avoid clutter. Keep important objects inside frame. No real logos, brands, watermarks, copyrighted characters, or unsupported claims.

## Motion
Smooth full-duration motion, meaningful intro/main/end, non-linear easing, restrained secondary motion, clean transitions. For loops, guarantee exact cycle continuity.

## Code contract
Output only JavaScript code.
Use:
function draw(ctx, time, width, height) { /* animation */ }

Rules:
- time in seconds
- responsive width/height
- Canvas API only
- no external libraries/assets/fonts
- controlled palette
- efficient frame-by-frame rendering
- no syntax errors
- deterministic seeded randomness when needed
- loop-safe when requested.