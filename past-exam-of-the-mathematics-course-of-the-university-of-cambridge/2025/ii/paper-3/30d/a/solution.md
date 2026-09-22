<h1 id="30d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the contour near the simple saddle as

$$
z=z_0+e^{i\alpha}s,\qquad s\in\mathbb R,
$$

with its given orientation. Since $\phi'(z_0)=0$,

$$
\phi(z)
=\phi(z_0)+\frac12\phi''(z_0)e^{2i\alpha}s^2
+O(s^3).
$$

Along a steepest-descent tangent the quadratic coefficient is real and negative, so

$$
\phi''(z_0)e^{2i\alpha}=-|\phi''(z_0)|,
\qquad
\arg\phi''(z_0)+2\alpha=\pi\pmod{2\pi}.
$$

Moreover $dz=e^{i\alpha}ds$. Only a neighbourhood of width $O(x^{-1/2})$ contributes at leading order, and there $f(z)=f(z_0)+o(1)$. The local integral is consequently

$$
f(z_0)e^{x\phi(z_0)+i\alpha}
\int_{-\infty}^{\infty}
\exp\left(-\frac{x|\phi''(z_0)|}{2}s^2\right)\,ds.
$$

Evaluating the Gaussian proves the [simple-saddle contribution in steepest descent](../../../../../../simple-saddle-contribution-in-steepest-descent.md):

$$
\boxed{
I(x)\sim
f(z_0)\sqrt{\frac{2\pi}{x|\phi''(z_0)|}}\,
e^{x\phi(z_0)+i\alpha}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [30D](../../30d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
