<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the same $h$, the squared [Hellinger distance](../../../../../../hellinger-distance.md) is

$$
d_H(f,\phi)^2=\frac12\int(h-1)^2d\gamma
=1-\int h\,d\gamma.
$$

Since $0\leq\int h\,d\gamma\leq1$,

$$
1-\int h\,d\gamma
\leq1-\left(\int h\,d\gamma\right)^2
=\operatorname{Var}_\gamma h.
$$

The [Gaussian Poincaré inequality](../../../../../../gaussian-poincare-inequality.md) and the derivative calculation in part (b) yield

$$
\boxed{d_H(f,\phi)^2\leq\frac14J(f\Vert\phi).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
