# Motion Scene Engineering — Layer 1

## Purpose

Build a precise scene and timeline specification for motion prompts.

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

Given a declared duration D:
- start at 0.00s
- allocate all meaningful time through D
- include entrance, action, transition, hold, and loop preparation where appropriate
- avoid arbitrary scene splitting
- avoid timeline gaps

## State-based thinking

Prefer state changes over vague descriptions.

Example pattern:
Initial → interaction → processing → success → hold → loop return.

The actual states must be adapted to the requested theme.

## Motion relationships

Distinguish:
- primary motion: the event that communicates the idea
- secondary motion: supporting movement
- micro motion: subtle life/polish
- transition motion: movement that changes one state to another

Primary motion should dominate.

## Timing hierarchy

Fast timing communicates interaction or emphasis.
Medium timing communicates transition.
Longer holds communicate comprehension.

Do not make every action equally fast.

## Keyframe summary

Use a compact checkpoint table when the animation is sufficiently complex.

Format:
Time | State | Primary Motion | Supporting Motion

## Loop engineering

For a loop:
- define the initial state precisely
- define the final state precisely
- ensure the transition path between them is intentional
- avoid relying on an unexplained fade unless that fade is the design

For procedural rendering, loop endpoints must be deterministic.

## Motion anti-slop

Reject motion added merely because the timeline feels empty.

Every movement must support comprehension, hierarchy, polish, or loop continuity.