INT6064 Coding and Computational Thinking — Semester 1, 2026-27
Individual Teaching Module (25%): Pedagogical Artifact / Codebase + Short Descriptive Paragraph
Student: WUPENGHUI (11729730)
Artifact: Particle Navigator — interactive physics simulation (Unity / C#)


====================================================================
DESCRIPTIVE PARAGRAPH
====================================================================
Particle Navigator is a simulation I built in Unity for a two-lesson module with my Secondary 4 physics class (ages 15-16). Students steer a charged particle into a receiver on the other side of the screen by choosing the magnetic field direction, and later the field strength and speed. I chose this because magnetic fields are invisible, and many students cannot see why the radius r = mv/(qB) makes the particle move in a circle. In Lesson 1 they predict which way the particle curves and check it with the left-hand rule, then use Level 1, where they can only change the direction. In Lesson 2 they change one variable at a time, collect speed, field and radius, and work out the radius rule themselves; then they plan a route across three field regions and try to find a second solution. A grey preview and the last attempt stay on screen, so students predict before they test and can see what changed. The computational thinking is in breaking the route into parts, treating the path as arcs, predicting and adjusting, debugging misses, and judging their own attempts. I should be honest about the limits: the solver is hidden and students mostly tune parameters rather than code, so I added a short optional Python or Scratch program where they predict the landing point, which links the model to real code.

====================================================================
WHAT IS IN THIS PACKAGE
====================================================================
01_Artifact/
  ChargeMotionLab.app/            Runnable macOS app (fully offline, no install).
  SourceCode/                    C# source of the module (ParticleNavigatorModule.cs).
  Screenshots/                   Key states: failure/success, the three levels,
                                 prediction path, and previous-vs-current trajectory.

02_TeacherNotes/
  INT6064 Individual Module - Teacher Notes - WUPENGHUI (docx/pdf)
                                 Deployment, lesson flow (2 lessons), scaffolding,
                                 differentiation, common issues and responses, assessment.
  ParticleNav_DeploymentGuide.md Detailed deployment guide and quick reference.

03_ShortDescription/
  INT6064 Individual Module - Artifact Description - WUPENGHUI (docx/pdf)
                                 The short descriptive paragraph (approx. 150-300 words).

04_TestResults/
  test_results.txt                    Self-test output (ParticleNavigatorModule.SelfTest()).

====================================================================
HOW TO RUN
====================================================================
- macOS: double-click 01_Artifact/ChargeMotionLab.app. It runs offline.
- Optional quick jump to the module (Terminal):
    open 01_Artifact/ChargeMotionLab.app --args -starthub -enterstation 4

====================================================================
HOW THIS MAPS TO THE RUBRIC (25%)
====================================================================
- Functionality & appropriateness (8):
    Working, runnable app for Secondary 4 physics (ages 15-16), matched to the
    learning objectives (magnetic force changes direction not speed; r = mv/(qB)).
- Evidence of CT development embedded (7):
    Three levels progress from choosing direction -> tuning radius -> designing a
    three-region route, deliberately building decomposition, abstraction,
    algorithmic prediction, debugging, evaluation and modelling into the artifact.
- Teacher notes / lesson materials (5):
    See 02_TeacherNotes (deployment, scaffolding, differentiation, common issues).
- Short descriptive paragraph (5):
    See 03_ShortDescription (approx. 150-300 words).

====================================================================
NOTES
====================================================================
- Platform justification: Unity/C# gives a real-time physics visualisation that a
  worksheet or Scratch cannot provide; the platform is used deliberately, not for
  technical show.
- Demo video and additional screenshots (for the separate 10% video component) are
  available in the original "第四站-粒子导航员" folder if required.
- Fully offline; no data is collected; the simulation resets to a new run on reopening.
