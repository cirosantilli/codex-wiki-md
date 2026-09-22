<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At fixed intrinsic ratio $q$, part a gives

$$
Q^2=q^2+(1-q^2)\mu^2,
\qquad
\mu=\sqrt{\frac{Q^2-q^2}{1-q^2}}.
$$

Since $\mu$ is uniform, the [change-of-variables formula for a probability density](../../../../../../change-of-variables-formula-for-a-probability-density.md) yields the conditional [probability density function](../../../../../../probability-density-function.md)

$$
\boxed{
\mathcal P(Q\mid q)
=\frac{d\mu}{dQ}
=\frac{Q}{\sqrt{1-q^2}\sqrt{Q^2-q^2}},
\qquad q\leq Q\leq1}.
$$

The inverse-square-root singularity at $Q=q$ is integrable, and direct integration gives one.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 320](../../../paper-320-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
