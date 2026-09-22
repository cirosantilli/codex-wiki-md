<h1 id="38b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Because the condition is local and covariant, choose [normal coordinates](../../../../../../normal-coordinates.md) at the point and a Lorentz frame in which the timelike observer is $X^\mu=\delta^\mu_0$. Rescaling a timelike vector by a positive factor does not affect the sign, so it suffices to use this unit vector. With signature $(-,+,\ldots,+)$,

$$
\nabla_\rho\phi\nabla^\rho\phi
=-(\partial_0\phi)^2+\sum_{i=1}^{D-1}(\partial_i\phi)^2.
$$

The measured energy density is therefore

$$
\begin{aligned}
2T_{\mu\nu}X^\mu X^\nu
=2T_{00}
&=(\partial_0\phi)^2
-A\left[-(\partial_0\phi)^2+\sum_i(\partial_i\phi)^2\right]
-B\phi^2\\
&=(1+A)(\partial_0\phi)^2
-A\sum_i(\partial_i\phi)^2-B\phi^2.
\end{aligned}
$$

The value of $\phi$, its time derivative, and its spatial first derivatives can be varied independently at a point. Nonnegativity for all such data is therefore equivalent to nonnegativity of all three coefficients:

$$
1+A\geq0,
\qquad
-A\geq0,
\qquad
-B\geq0.
$$

Thus the most general constraints are

$$
\boxed{-1\leq A\leq0,
\qquad B\leq0}.
$$

These conditions are also sufficient in every timelike frame, because any timelike vector can be brought to the chosen rest frame. This is the [weak energy condition for a quadratic scalar stress-energy ansatz](../../../../../../weak-energy-condition-for-a-quadratic-scalar-stress-energy-ansatz.md).

The conserved values from part (a),

$$
A=-\frac12,
\qquad
B=-\frac{m^2}{2},
$$

satisfy these inequalities for real $m$, as required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [38B](../../38b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
