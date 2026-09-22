<h1 id="14e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $|z|<1$ on the negative-real portions of the [Hankel contour](../../../../../../hankel-contour.md), expand

$$
\frac{z}{e^{-t}-z}=\frac{ze^t}{1-ze^t}
=\sum_{n\geq1}z^ne^{nt}.
$$

Local uniform convergence permits termwise integration. The reciprocal Hankel formula gives

$$
\frac1{2\pi i}\int_{-\infty}^{(0+)}e^{nt}t^{s-1}dt
=\frac{n^{-s}}{\Gamma(1-s)},
$$

so $I(z,s)=\sum_{n\geq1}z^n/n^s=\operatorname{Li}_s(z)$ initially on the disc.

For $z\notin[1,\infty)$, choose the contour around the negative axis so that it passes between zero and every pole satisfying $e^{-t}=z$. On compact subsets of the slit $z$-plane it can be chosen uniformly, and differentiation under the integral proves holomorphy. Deforming without crossing a pole gives a single-valued analytic continuation. Near the cut, the pole $t=-\log z$ lies on opposite sides of the two admissible contours; this is why the contour must pass it consistently.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [14E](../../14e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
