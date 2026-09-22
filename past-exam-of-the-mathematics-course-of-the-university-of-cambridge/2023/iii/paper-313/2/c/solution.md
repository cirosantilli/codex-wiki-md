<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a rotationally symmetric vortex, the equation away from the origin is

$$
u''+\frac1r u'=e^u-1.
$$

Insert

$$
u=\alpha\log r+\beta+\gamma r+\delta r^2+\cdots.
$$

The prescribed zero fixes $\alpha=2N$. Since $N\geq1$, $e^u=e^\beta r^{2N}[1+o(1)]$, while

$$
u''+\frac1r u'=\frac\gamma r+4\delta+o(1).
$$

Matching the singular and constant terms with $e^u-1=-1+o(1)$ gives

$$
\boxed{(\alpha,\gamma,\delta)=\left(2N,0,-\frac14\right)}.
$$

The undetermined $\beta$ is fixed by matching this local expansion to $u\to0$ at infinity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 313](../../../paper-313-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
