<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the sign convention

$$
\mathcal L(x,z)=f(x)-z^T(Ax-b)
$$

for the [Lagrangian function in constrained optimization](../../../../../../lagrangian-function-in-constrained-optimization.md). The [Lagrangian dual problem](../../../../../../lagrangian-dual-problem.md) is

$$
\boxed{
\max_{z\in\mathbb R^m}q(z),
\qquad
q(z)=\inf_x\mathcal L(x,z)
=b^Tz-f^*(A^Tz),}
$$

where $f^*$ is the [convex conjugate](../../../../../../convex-conjugate.md). For this convex problem with affine equality constraints, the stationarity and feasibility parts of the [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) are

$$
\nabla f(x)-A^Tz=0,
\qquad Ax-b=0.
$$

They say exactly that the displayed operator satisfies

$$
\boxed{
F\binom{x}{z}
=\binom{\nabla f(x)-A^Tz}{Ax-b}=0.}
$$

Thus its zeros are precisely the [primal-dual optimal points](../../../../../../primal-dual-optimal-point.md), subject to the usual attainment assumptions.

For $u=(x,z)$ and $\widetilde u=(y,s)$, the [Euclidean inner product](../../../../../../inner-product.md) gives

$$
\begin{aligned}
\langle F(u)-F(\widetilde u),u-\widetilde u\rangle
={}&\langle\nabla f(x)-\nabla f(y),x-y\rangle\\
&-\langle A^T(z-s),x-y\rangle
+\langle A(x-y),z-s\rangle.
\end{aligned}
$$

The last two terms cancel by the defining property of the [matrix transpose](../../../../../../transpose.md), and the first is nonnegative by part a. Hence $F$ is a [monotone operator](../../../../../../monotone-operator.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
