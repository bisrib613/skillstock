# Stock Production & QA — Layer 1

## Purpose
Validate the prompt against the commercial framework, premium quality requirements, technical direction, compliance constraints, and source-template contract. This is prompt QA, not actual rendering.

## Demand QA
Confirm:
- buyer/use case is identifiable;
- visual utility is explicit;
- concept is connected to a supported market need, evergreen need, current opportunity, or clearly marked inference;
- saturated literal metaphors were avoided or functionally transformed;
- no sales/ranking guarantee is claimed.

## Premium QA
Check:
- hierarchy and focal point are clear;
- composition supports the buyer use case;
- copy space/isolation is used when useful, not mechanically;
- palette and depth are coherent;
- asset is modular/adaptable where the use case benefits;
- motion uses purposeful non-linear timing and restrained secondary motion when animated;
- detail improves implementation rather than padding prose.

## Technical vector QA
When vector is relevant:
- closed paths;
- clean curves/node density;
- expanded strokes/outlined text where required;
- no embedded raster for pure vector;
- no auto-trace artifacts;
- logical layer/group structure;
- consistent perspective/lighting.

## Motion QA
When motion is relevant:
- duration is one of the project-approved choices;
- timeline starts at 0.00s and ends exactly at declared duration;
- no overlaps or unexplained gaps;
- important states fit the runtime;
- easing and motion hierarchy are explicit;
- loop endpoints are deterministic when looping.

## Programmatic QA
When code-generated:
- deterministic procedural behavior;
- stable frame state;
- resolution-independent layout;
- font readiness where applicable;
- bounded rendering complexity;
- no uncontrolled asynchronous dependencies.

## Failure-pattern gate
Reject or revise prompts showing:
- visual noise/over-decoration;
- generic saturated metaphors;
- messy auto-trace/geometry;
- inconsistent perspective or lighting;
- robotic linear motion;
- anatomy/hardware distortion risk when applicable;
- metadata/variation spam encouragement.

## Marketplace/IP QA
Keep universal IP safety in the prompt. Treat platform-specific submission rules as time-sensitive and destination-specific.
Do not claim a marketplace will accept or reject an asset without current platform evidence.

## Template fidelity
Preserve the source role statement, fields, order, fixed values, fixed rule blocks, and user overrides. Resolve only open fields and insert enrichment only where the template permits it.

## Output
Return the completed prompt, not the QA checklist, unless the user asks for the audit.
