# Motion Scene Engineering — Layer 1

## Purpose
Build a precise scene, state, and timeline architecture for professional motion prompts.

## No preset duration or scene count
Do not assume a fixed runtime or scene count.
Determine duration and number of scenes from explicit user constraints first, then from commercial use, concept complexity, readability, and loop requirements.

This project uses 5, 10, or 15 seconds as the standard motion durations. Choose 5, 10, or 15 internally based on the concept, commercial use case, scene complexity, readability, and loop requirements. Do not import another duration from an example or previous conversation unless the user explicitly requests it.

One scene at 5 seconds is valid when the concept communicates better that way. A longer duration or multiple scenes is valid when the concept requires it.

## Scene model
For each scene/state define:
- time range
- purpose
- visible elements
- starting state
- primary action
- supporting motion
- transition
- ending state

## Timeline construction
Given the selected duration:
- start at 0.00s
- end exactly at the selected duration
- do not overlap ranges
- do not leave unexplained gaps
- include transitions and holds
- use the full runtime intentionally

## State-based thinking
Prefer meaningful state changes over vague descriptions.

Example pattern:
initial → interaction → processing → success → hold → loop return

Adapt the pattern to the requested concept.

## Motion hierarchy
Primary motion communicates the idea.
Secondary motion supports the primary event.
Micro motion adds polish.
Transition motion changes state.

Do not let micro motion compete with primary motion.

## Timing hierarchy
Use faster timing for emphasis or interaction, medium timing for transformation, and longer holds where comprehension benefits.

Do not make every action equally fast.

## Keyframe summary
When the animation has meaningful complexity, include:
Time | State | Primary Motion | Supporting Motion

## Loop engineering
When a loop is requested, precisely describe the initial state, final state, return path, and deterministic relationship between the endpoints.

Do not rely on unexplained fades as the only loop strategy unless that is intentionally part of the concept.

## Anti-slop
Reject movement added only because the timeline feels empty.
Every motion should serve comprehension, hierarchy, polish, interaction, or loop continuity.