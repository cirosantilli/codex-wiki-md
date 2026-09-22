<h1 id="26j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a unit-speed space curve, set

$$
t=\dot\alpha,\qquad
\kappa=|\dot t|,\qquad
n=\frac{\dot t}{\kappa},\qquad b=t\times n.
$$

These form the Frenet trihedron. With the signed torsion convention compatible with the question, the [Frenet-Serret formulas](../../../../../../frenet-serret-formulas.md) are

$$
\dot t=\kappa n,\qquad
\dot n=-\kappa t-\tau b,\qquad
\dot b=\tau n.
$$

For an oriented surface with [unit normal](../../../../../../unit-normal.md) $N$, the signed [geodesic curvature](../../../../../../geodesic-curvature.md) is

$$
\kappa_g=\langle\dot t,N\times t\rangle.
$$

On the unit sphere $N=\alpha$. Since $\alpha\cdot t=0$, [differentiation](../../../../../../differentiation.md) gives

$$
1+\kappa\,\alpha\cdot n=0.
$$

Write $\alpha=An+Bb$. Then $A=-1/\kappa$, and differentiating this expression and comparing the $n$ coefficient with $\dot\alpha=t$ gives

$$
\dot A+\tau B=0,\qquad
B=-\frac{\dot\kappa}{\tau\kappa^2}.
$$

Thus, wherever the displayed quantities are defined,

$$
\boxed{\alpha=-\kappa^{-1}n-\tau^{-1}\kappa^{-2}\dot\kappa\,b}.
$$

Finally,

$$
\kappa_g
=\kappa n\cdot(\alpha\times t)
=-\frac{\dot\kappa}{\tau\kappa},
$$

which is the stated [curvature decomposition for a spherical curve](../../../../../../curvature-decomposition-for-a-spherical-curve.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26J](../../26j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
