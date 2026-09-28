# Motion Scene Engineering — Layer 1

## Purpose
Build scene/state architecture that supports commercial comprehension and downstream implementation.

## Duration and scene count
No preset duration or scene count.
Choose only 5, 10, or 15 seconds for the active project, based on:
commercial use → communication complexity → meaningful states → readability → loop/ending needs.
Never copy a duration from a research example; research examples may contain other values.

## Scene/state model
For each meaningful scene/state define:
- time range;
- purpose;
- visible elements;
- starting state;
- primary action;
- supporting motion;
- transition;
- ending state.

## Timeline
- start at 0.00s;
- end exactly at selected duration;
- no overlap;
- no unexplained gaps;
- transitions and holds are intentional;
- primary communication beat receives enough readable time.

## Motion hierarchy
Primary motion communicates the message.
Secondary motion supports it.
Micro motion adds polish.
Transition motion changes state.
Remove motion that serves none of comprehension, hierarchy, polish, interaction, or loop continuity.

## Research-derived pacing
Research identifies linear mechanical interpolation as a quality weakness. Use acceleration/deceleration, custom cubic-bezier or spring-like behavior, settling, and restrained secondary motion where appropriate.
Do not force non-linear easing when constant speed is functionally correct.

## Commercial motion patterns
Useful patterns include:
- workflow/process reveal;
- verification/status change;
- dashboard/data update;
- infrastructure/data flow;
- isolated UI/overlay interaction;
- transformation/comparison;
- seamless loop.

Select the pattern from buyer use case, not a preset.

## Keyframe summary
For meaningful complexity:
Time | State | Primary Motion | Supporting Motion

## Loop engineering
When looping, specify initial state, final state, deterministic return path, and endpoint equivalence. Do not use an unexplained fade as the default loop solution.

## Anti-slop
Never add motion merely to fill empty runtime.
