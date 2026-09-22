<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the [Lorentz transformation](../../../../lorentz-transformation.md) as $x'^\mu=\Lambda^\mu{}_{\nu}x^\nu$. Acting on a [scalar field](../../../../scalar-field.md), the [chain rule](../../../../chain-rule.md) gives the [four-gradient](../../../../four-gradient.md)

$$
\partial'_\mu=\frac{\partial x^\nu}{\partial x'^\mu}\partial_\nu
=(\Lambda^{-1})^\nu{}_{\mu}\partial_\nu.
$$

For the specified [Lorentz boost](../../../../lorentz-boost.md), the inverse is obtained by changing $\beta$ to $-\beta$, so

$$
\partial'_0=\gamma(\partial_0+\beta\partial_1),\qquad
\partial'_1=\gamma(\partial_1+\beta\partial_0),\qquad
\partial'_2=\partial_2,\quad\partial'_3=\partial_3.
$$

These are precisely the [covector](../../../../covector.md) component rules for the lowered coordinates. Raising the index with the [Minkowski metric](../../../../minkowski-metric.md) $\eta^{\mu\nu}=\operatorname{diag}(-1,1,1,1)$ reverses the time component, yielding

$$
\boxed{\partial_\mu=(c^{-1}\partial_t,\partial_x,\partial_y,\partial_z),\qquad
\partial^\mu=(-c^{-1}\partial_t,\partial_x,\partial_y,\partial_z).}
$$

Indeed $\partial'^0=\gamma(\partial^0-\beta\partial^1)$ and $\partial'^1=\gamma(\partial^1-\beta\partial^0)$, the contravariant [four-vector](../../../../four-vector.md) rules. Thus the index on a [partial derivative](../../../../partial-derivative.md) with respect to an upper coordinate is lower.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
