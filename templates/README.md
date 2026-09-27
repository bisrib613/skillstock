# Templates

## Active Layer 1
`motion-canvas-js-to-mp4-prompt.md` is the canonical user-supplied Motion Studio prompt template.

Layer 1 fills and enriches this prompt but does not execute it.

## Parameter policy
The active template has no hardcoded duration, scene count, aspect ratio, resolution, FPS, or loop default.

Only Vector and Flat vector remain explicitly fixed in the supplied template.

All other production parameters are reasoned internally from the user request, commercial use case, concept, and relevant skills.

## Template handling
The source template's role, fields, fixed values, and fixed instruction blocks are preserved.
Generated production-specification detail may be inserted between the settings/concept area and the fixed ATURAN blocks when needed for a professional result.

## Future Layer 2
Files under `future/layer-2/` are archived for later downstream code-generation work.
They are not active in the current prompt-building layer.