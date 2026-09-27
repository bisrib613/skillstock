# Motion Art Direction — Prompt Specification

## Purpose

Translate a commercial concept into motion direction detailed enough for a downstream renderer or animator.

A premium motion prompt must describe not only what is visible, but how the visual state changes over time.

## Motion design stack

For animated prompts, define when relevant:
1. scene/state purpose
2. visual state at entry
3. primary action
4. supporting or micro movement
5. transition method
6. visual state at exit
7. timing range
8. easing/velocity character
9. hold/settling behavior
10. loop relationship when looping is requested

## Timeline

Use explicit time ranges when duration is known.

Scene ranges must:
- begin at 0.00s
- end at the declared duration
- not overlap
- not leave unexplained gaps
- include transitions and holds
- use the meaningful duration of the asset

Primary timeline units are seconds.

## Keyframes

For important state changes, provide:
time → state → primary motion → supporting motion

Do not specify every trivial movement. Keyframes should make the animation reproducible and understandable.

## Easing

Choose easing by behavior:
- entrance/exit → appropriate acceleration/deceleration and settling
- UI press/release → short responsive ease-in-out
- morph/state transition → custom cubic or spring-like behavior
- progress/process indicators → consistent timing when functional
- reveal/success → controlled overshoot or draw-on when useful

Avoid linear motion when the desired behavior is physical or tactile, unless constant speed is functionally appropriate.

## Motion language

Prefer anticipation, acceleration/deceleration, settling, restrained secondary motion, micro-motion, readable staging, and clear state changes.

Avoid random motion, excessive particles, unnecessary camera movement, unreadable rapid sequencing, and effects that compete with the communication goal.

## Loop

When looping is requested, describe how the ending returns to the initial state without visible discontinuity.

For code/frame rendering, loop behavior must be deterministic.

## Commercial utility

Motion should communicate a process, state, interaction, transformation, status, or useful visual system.

Do not turn every stock clip into a spectacle merely to fill time.