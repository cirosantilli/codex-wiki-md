<h1 id="s/s2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**State-dependent execution times can [bias](../../../../../bias-of-an-estimator.md) the finite set of completed outputs.** A simple counterexample takes $p=q$ uniform on two states and $M=1$, so every proposal is accepted. Suppose processing the first state takes one unit of time and processing the second takes two. Stop at a [deadline](../../../../../deadline-truncation-bias-in-rejection-sampling.md) between one and two units, discarding any unfinished computation. The only possible completed output is the first state; conditional on obtaining a sample, its law is concentrated there rather than uniform.

This demonstrates that a wall-clock cutoff can select outputs according to their processing cost, unlike the fixed proposal budget in (d). It does not imply a permanent asymptotic [bias](../../../../../bias-of-an-estimator.md) of averages over an indefinitely growing completed sequence: the finite-horizon stopping and censoring are the issue. Without assumptions relating runtime to states, exact finite-sample unbiasedness cannot be guaranteed.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [S2](../../s2.md)
3. [S](../../../s.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
