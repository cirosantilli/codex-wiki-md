<h1 id="s31/3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

An [explicit numerical method](../../../../../explicit-numerical-method.md) normally has a simple, inexpensive step and needs no simultaneous solve, but stability can force very small steps, especially for [stiff differential equations](../../../../../stiff-equation.md). An [implicit numerical method](../../../../../implicit-numerical-method.md) requires a linear or nonlinear solve, storage and suitable solver tolerances; its larger stability region can permit larger steps when stability is the main restriction. Accuracy, phase fidelity and preservation of physical structure still constrain the step. For this [oscillator](../../../../../oscillator.md), backward [Euler method](../../../../../euler-method.md) is stable but dissipative, while forward [Euler method](../../../../../euler-method.md) is cheap but unstable without damping. Neither statement makes all implicit methods superior to all explicit ones; method order, problem structure and total cost determine the useful choice.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [S31](../../../s31.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
