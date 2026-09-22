<h1 id="33d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The system prescribes both first derivatives of the same vector $\psi$, so it is overdetermined: the two mixed derivatives must agree. Differentiating gives

$$
\begin{aligned}
\partial_{\bar z}\partial_z\psi
&=(\partial_{\bar z}U)\psi+U\partial_{\bar z}\psi
=(\partial_{\bar z}U+UV)\psi,\\
\partial_z\partial_{\bar z}\psi
&=(\partial_zV)\psi+V\partial_z\psi
=(\partial_zV+VU)\psi.
\end{aligned}
$$

Thus every solution satisfies

$$
\left(
\partial_{\bar z}U-\partial_zV+[U,V]
\right)\psi=0.
$$

For the system to possess arbitrary nontrivial local solution data, the coefficient matrix must vanish:

$$
\boxed{\partial_{\bar z}U-\partial_zV+[U,V]=0}.
$$

This is the [zero-curvature condition](../../../../../../zero-curvature-condition.md), or the [compatibility condition for an overdetermined linear system](../../../../../../compatibility-condition-for-an-overdetermined-linear-system.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [33D](../../33d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
