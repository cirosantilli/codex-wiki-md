<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $s<t$, write $X_t=X_s+Y$, where the increment $Y=X_t-X_s$ is independent of the [natural filtration](../../../../../../natural-filtration.md) at time $s$, has mean zero, and has variance $(t-s)\sigma^2$. Hence

$$
\mathbb E[X_t^2\mid\mathcal F_s]
=X_s^2+\mathbb E[Y^2]
=X_s^2+(t-s)\sigma^2.
$$

It follows that $M_t=X_t^2-t\sigma^2$ is a martingale, as asserted by the [centered square-integrable Lévy martingale](../../../../../../centered-square-integrable-levy-martingale.md) identity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
