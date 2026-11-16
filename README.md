# Particle Navigator

**INT6064 Coding and Computational Thinking** — Semester 1, 2026-27
Individual Teaching Module (25%): Pedagogical Artifact / Codebase + Short Descriptive Paragraph

**Student:** WUPENGHUI (11729730)
**Artifact:** Particle Navigator — interactive physics simulation (Unity / C#)

## Descriptive Paragraph

Particle Navigator is a simulation I built in Unity for a two-lesson module with my Secondary 4 physics class (ages 15-16). Students steer a charged particle into a receiver on the other side of the screen by choosing the magnetic field direction, and later the field strength and speed. I chose this because magnetic fields are invisible, and many students cannot see why the radius r = mv/(qB) makes the particle move in a circle. In Lesson 1 they predict which way the particle curves and check it with the left-hand rule, then use Level 1, where they can only change the direction. In Lesson 2 they change one variable at a time, collect speed, field and radius, and work out the radius rule themselves; then they plan a route across three field regions and try to find a second solution. A grey preview and the last attempt stay on screen, so students predict before they test and can see what changed. The computational thinking is in breaking the route into parts, treating the path as arcs, predicting and adjusting, debugging misses, and judging their own attempts. I should be honest about the limits: the solver is hidden and students mostly tune parameters rather than code, so I added a short optional Python or Scratch program where they predict the landing point, which links the model to real code.

## What's here

- `ParticleNavigatorModule.cs` — the C# source of the Particle Navigator module.
- `screenshots/` — key states: failure/success, the three levels, the prediction path, and the previous-vs-current trajectory.
- The runnable macOS app and teacher notes are part of the full module package.

## How to run

- macOS: open `ChargeMotionLab.app` (from the full package); it runs fully offline.
- Optional quick jump (Terminal): `open ChargeMotionLab.app --args -starthub -enterstation 4`

## How this maps to the rubric (25%)

- **Functionality & appropriateness (8):** a working, runnable app for Secondary 4 physics (ages 15-16), matched to the learning objectives (magnetic force changes direction not speed; r = mv/(qB)).
- **Evidence of CT development embedded (7):** three levels progress from choosing direction, to tuning the radius, to designing a three-region route — building decomposition, abstraction, algorithmic prediction, debugging, evaluation and modelling into the artifact.
- **Teacher notes / lesson materials (5):** deployment, lesson flow, scaffolding, differentiation, common issues and responses, assessment.
- **Short descriptive paragraph (5):** see the paragraph above.

## Notes

- Unity/C# gives a real-time physics visualisation that a worksheet or Scratch cannot; the platform is used deliberately, not for technical show.
- Fully offline; no data is collected; the simulation resets to a new run on reopening.
