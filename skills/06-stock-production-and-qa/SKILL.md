# Stock Production & QA — Layer 1

## Purpose
Validate the prompt against commercial demand, premium quality, technical direction, compliance constraints, and source-template fidelity. This is prompt QA, not actual rendering.

## Demand QA
Confirm:
- buyer/use case is identifiable;
- visual utility is explicit;
- concept connects to a supported market need, evergreen need, current opportunity, or clearly marked inference;
- saturated literal metaphors were avoided or functionally transformed;
- no sales/ranking guarantee is claimed;
- for Auto Concept, the concept was generated from reasoning over research-derived signals rather than copied from a fixed topic list;
- Auto Concept candidates are materially distinct and not an identical/recycled set.

## Premium QA
Check hierarchy, focal point, buyer-appropriate composition, useful copy space/isolation, coherent palette/depth, modularity where useful, and purposeful motion. Detail must reduce implementation ambiguity rather than pad prose.

## Vector QA
When relevant:
- closed paths;
- clean curves/node density;
- expanded strokes/outlined text where required;
- no embedded raster in pure vector;
- no auto-trace artifacts;
- logical layer/group structure;
- consistent perspective/lighting.

## Motion QA
When relevant:
- duration is one of project-approved choices;
- timeline starts 0.00s and ends exactly at declared duration;
- no overlap or unexplained gap;
- important states fit runtime;
- easing and motion hierarchy are explicit;
- loop endpoints are deterministic.

## Programmatic QA
When code-generated:
- deterministic procedural behavior;
- stable frame state;
- resolution-independent layout;
- font readiness where applicable;
- bounded rendering complexity;
- no uncontrolled asynchronous dependencies.

## Failure-pattern gate
Reject/revise prompts showing:
- visual noise/over-decoration;
- generic saturated metaphors;
- messy auto-trace/geometry;
- inconsistent perspective/lighting;
- robotic linear motion;
- anatomy/hardware distortion risk where applicable;
- metadata or near-duplicate spam encouragement.

## Marketplace/IP QA
Keep universal IP safety in the prompt. Treat platform-specific submission rules as time-sensitive and destination-specific. Do not claim acceptance/rejection without current evidence.

## Template fidelity
Preserve source role statement, fields, order, fixed values, fixed rule blocks, and user overrides. Resolve only open fields and insert enrichment only where permitted.

## Output
Return the completed prompt, not the QA report, unless explicitly requested.
