<h1 id="15c/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $Q=2^m$. Applying the transform term by term gives

$$
|\phi_2\rangle
=\frac1{\sqrt{AQ}}\sum_{u=0}^{Q-1}
\sum_{j=0}^{A-1}e^{2\pi i(x_0+jr)u/Q}|u\rangle
=\sum_{u=0}^{Q-1}g(u)|u\rangle,
$$

where

$$
\boxed{
g(u)=\frac{e^{2\pi i x_0u/Q}}{\sqrt{AQ}}
\sum_{j=0}^{A-1}e^{2\pi i jru/Q}.}
$$

Thus, when $e^{2\pi iru/Q}\ne1$,

$$
\boxed{
g(u)=\frac{e^{2\pi i x_0u/Q}}{\sqrt{AQ}}
\frac{1-e^{2\pi iAru/Q}}{1-e^{2\pi iru/Q}}.}
$$

If the denominator vanishes, the continuous limiting value is

$$
g(u)=\sqrt{A/Q}\,e^{2\pi ix_0u/Q}.
$$

The magnitude is a Dirichlet-kernel peak near integers $u$ for which $ru/Q$ is close to an integer.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [15C](../../../15c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
