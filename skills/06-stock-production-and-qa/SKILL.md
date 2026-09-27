# Prompt Production & QA — Layer 1

## Purpose

Validate the completed production prompt before it is returned.

This is prompt QA only. It does not render or test the downstream asset.

## Completeness gate

For a premium motion prompt, verify that the prompt contains or clearly determines, when relevant:
- theme and commercial purpose
- buyer/use case
- visual concept
- visual style
- palette or color roles
- composition/framing
- subject hierarchy
- scene structure
- explicit timeline
- motion behavior
- easing/timing guidance
- key visual states
- loop behavior when requested
- technical constraints
- IP/brand restrictions
- downstream output contract

A prompt that merely restates the theme and a few generic style words is not complete.

## Timeline QA

Confirm:
- first scene starts at 0.00s
- final scene ends at the declared duration
- ranges do not overlap
- no unexplained gaps
- transitions are represented
- important beats fit inside the runtime
- loop preparation is accounted for when looping is requested

## Internal consistency

Check:
- style matches concept
- composition matches buyer/use case
- palette supports hierarchy
- motion supports comprehension
- technical rules do not contradict creative direction
- loop instructions fit the declared timeline
- explicit user choices remain unchanged

## Premium-depth QA

For a motion prompt, check that the specification is implementation-ready rather than decorative prose.

Look for:
- concrete state changes
- approximate timing for meaningful actions
- motion behavior and easing
- composition/framing guidance
- visual hierarchy
- restrained supporting motion
- a clear ending/hold
- a coherent loop strategy when requested

Do not invent arbitrary measurements simply to make the prompt longer.

## Template fidelity QA

Confirm:
- original role statement preserved
- original field names preserved
- original populated defaults preserved unless explicitly overridden
- original fixed rule blocks preserved
- intentionally blank fields resolved
- generated enrichment does not replace or reorder original fixed sections
- no downstream code was generated

## Commercial QA

Check for:
- functional visual utility
- differentiation from known saturation risks
- unnecessary decoration
- unclear hierarchy
- weak buyer context
- unsupported factual claims
- unnecessary brand/IP exposure

## Output discipline

Return the completed prompt, not this QA report, unless the user explicitly asks to see the audit.