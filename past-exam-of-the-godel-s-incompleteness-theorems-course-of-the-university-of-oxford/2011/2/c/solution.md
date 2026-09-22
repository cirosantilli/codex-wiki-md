<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use just the assumed local reflection instance with $Y=\neg X$:

$$
S+\{X\}\vdash B_S(\neg X)\to\neg X.
$$

By the [deduction theorem for propositional logic](../../../../deduction-theorem-for-propositional-logic.md), $S\vdash X\to(B_S(\neg X)\to\neg X)$. [Classical propositional logic](../../../../classical-propositional-logic.md) makes this imply the unconditional reflection statement $S\vdash B_S(\neg X)\to\neg X$: if $X$ is false the consequent is already true, and if $X$ is true the displayed implication supplies it. [Löb's theorem](../../../../lob-s-theorem.md) applied to $\neg X$ now gives

$$
\boxed{S\vdash\neg X.}
$$

Thus [full local reflection in a one-sentence extension is inconsistent](../../../../full-local-reflection-in-a-one-sentence-extension-is-inconsistent.md); in this argument even the single instance concerning $\neg X$ suffices.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Gödel's incompleteness theorems course of the University of Oxford](../../../split.md)
5. [Gödel's incompleteness theorems course of the University of Oxford](../../../../godel-s-incompleteness-theorems-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
